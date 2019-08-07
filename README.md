# eks
### Deployment Process : 

```mermaid
graph TD;
  CREATE_VM-->AW_ACCOUNT ;
  CREATE_EKS-->AW_ACCOUNT;
  AW_ACCOUNT-->DEPLOY_SCRIPT;
  DEPLOY_SCRIPT-->K8S_CLIENT;
  DEPLOY_SCRIPT-->HELM_CLIENT;
```

#lunch . stack 
```
aws cloudformation deploy --template template.yaml --stack-name my-new-stack --parameter-overrides Key1=Value1 Key2=Value2
```
