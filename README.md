# Laboratorio 11 - Infraestructura Big Data como Código

## Universidad César Vallejo

Curso: Business Intelligence and Big Data

## Descripción

Implementación de una infraestructura Big Data mediante
Terraform y Floci, utilizando servicios AWS emulados localmente.

## Herramientas

- Docker Desktop
- Terraform
- Floci
- AWS CLI
- Git y GitHub
- Visual Studio Code

## Recursos implementados

- Bucket S3: ucv-data-platform.
- Dominios: sales, customers, products y marketing.
- Capas: Bronze, Silver y Gold.
- Cuatro bases de datos Glue Data Catalog.

## Ejecución

1. docker compose up -d
2. cd terraform
3. terraform init
4. terraform validate
5. terraform plan
6. terraform apply

## Eliminación

terraform destroy

## Nota

Se utiliza lifecycle ignore_changes en las etiquetas de
Glue debido a las diferencias detectadas en el emulador Floci.

## Conclusión

Terraform permite crear, modificar y eliminar infraestructura
de manera automatizada y reproducible.