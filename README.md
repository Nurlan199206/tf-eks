# tf-eks
Deploy new AWS EKS cluster

##Terraform v1.0.1

```brew install awscli```

```aws configure```


```AWS Access Key ID [None]: YOUR_AWS_ACCESS_KEY_ID```

```AWS Secret Access Key [None]: YOUR_AWS_SECRET_ACCESS_KEY```

```Default region name [None]: YOUR_AWS_REGION```

```Default output format [None]: json```









```terraform init```

```terraform apply```








```aws eks --region $(terraform output -raw region) update-kubeconfig --name $(terraform output -raw cluster_name)``` or use generated kubeconfig file
