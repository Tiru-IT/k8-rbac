OpenID connect create
```
eksctl utils associate-iam-oidc-provider --cluster roboshop-dev --approve
```

eksctl create iamserviceaccount --cluster roboshop-dev --name secret-reader --namespace roboshop --attach-policy-arn arn:aws:iam::194796552797:policy/RoboShopMySQLSeceretReader --approve
