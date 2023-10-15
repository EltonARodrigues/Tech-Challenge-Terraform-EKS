# Tech Challenge - Pós-Tech SOAT - FIAP - Terraform EKS

Deploy do ambiente EKS da AWS para o projeto [Tech Challenge](https://github.com/diorgeneseugenio/fiap-tech-challenge-soat)


## Deploy

``` 
terraform init
terraform plan -out tfplan
terraform apply tfplan

# Destruir

terraform destroy
```

Árvore do projeto:
```bash
.
├── modules
│   ├── eks
│   │   ├── cluster.tf
│   │   ├── output.tf
│   │   └── variable.tf
│   └── network
│       ├── output.tf
│       ├── variable.tf
│       └── vpc.tf
├── modules.tf
├── output.tf
├── provider.tf
├── README.md
└── variable.tf # variaveis do ambiente
```