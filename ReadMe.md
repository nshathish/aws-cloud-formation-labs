### deploy stack (create and update)
(if an existing stack name is given, it will update the stack)

```yaml
aws cloudformation deploy --template-file /path_to_template/template.json --stack-name my-new-stack --parameter-overrides Key1=Value1 Key2=Value2 --tags Key1=Value1 Key2=Value2
```