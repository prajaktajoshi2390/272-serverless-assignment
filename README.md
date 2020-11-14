Serverless Implementation with AWS
- Problem Statement: Detect image having Cat and remove image from bucket if no Cat present.
- Technology Stack:
-- Serverless Framework
-- AWS (Rekognition, S3, Lambda)
-- NodeJS
- Application Workflow:
This application uses serverless framework to detect images having Cat. When any image is uploaded to Amazon S3, corresponding Lambda event triggers. Amazon Rekognition API generates labels for the uploaded image. Handler function filters images based on the label named ‘Cat’. Images having Cat remain in S3 bucket while images without Cat get deleted from S3 bucket. 
