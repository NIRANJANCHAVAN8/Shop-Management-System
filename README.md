# Shop Management System
Serverless shop manager: S3 (frontend) + API Gateway + Lambda (Python) + DynamoDB, deployed by GitHub Actions with AWS SAM.

## API (send header `x-api-key`)
- GET/POST /products, PUT/DELETE /products/{id}
- POST /sales  body: {"items":[{"product_id":"...","qty":2}]}
- GET /sales, GET /reports/low-stock

## Local test
pip install -r requirements-dev.txt && pytest
