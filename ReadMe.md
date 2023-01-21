### deploy stack (create and update)
(if an existing stack name is given, it will update the stack)

```bash
aws cloudformation deploy ^
    --template-file /path_to_template/template.json ^
    --stack-name my-new-stack ^
    --parameter-overrides Key1=Value1 Key2=Value2 ^
    --tags Key1=Value1 Key2=Value2
```

### create-stack

```bash
aws cloudformation create-stack ^
    --stack-name packt-chap1-1 ^
    --template-body file://packt-mastering-cloudformation/chap1.yml
```

### update-stack
```bash
aws cloudformation update-stack ^
    --stack-name packt-chap1 ^
    --template-body file://packt-mastering-cloudformation/chap1.yml

```


### delete-stack
```bash
aws cloudformation delete-stack --stack-name packt-chap1

```

_^ is the symbol to break command into multiple lines (equivalent of \ in *nix systems)_

_To log into EC2 using ssh, the keys are in .aws/keys folder; connect to EC2 from that folder; this way no need to configure chmod in windows_