# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Encrypted catalogue and sales imports, checked on arrival |
| Bedrock | Product classification from catalogue text |
| SageMaker AI | Category sales forecasts, retrained monthly |
| DynamoDB | Categories, suggestions and buyer decisions |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
