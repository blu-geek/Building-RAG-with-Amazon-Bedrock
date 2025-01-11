# Building-RAG-with-Amazon-Bedrock

Building a RAG-Enhanced Knowledge Management System with Amazon Bedrock using Knowledge Bases

As a Generative AI Developer at Valtara you are tasked with enhancing the efficiency and intelligence of your company's knowledge management system to support internal teams and improve customer support. Leveraging Amazon Bedrock Knowledge Bases in conjunction with Retrieval-Augmented Generation (RAG), you aim to create an intelligent, scalable knowledge repository capable of Valtara providing quick and accurate answers to queries from internal stakeholders and customers. By integrating RAG with Amazon Bedrock Knowledge Bases, you streamline information retrieval processes and augment generative responses, ensuring that employees and clients have access to up-to-date and relevant information, which leads to improved productivity and customer satisfaction. 

# Retrieval Augmentation and Generation (RAG)





<img width="710" alt="Screenshot 2025-01-10 at 21 12 35" src="https://github.com/user-attachments/assets/1a4e2734-6c1c-4b58-9d95-a72f1c4c4041" />





# Activity Guide: Building a RAG-Enhanced Knowledge Management System with Amazon Bedrock

1. Set Up the AWS Environment
Create IAM User:
Ensure you have an IAM user with Administrator Access.
Enable Bedrock Foundation Models:
Activate Bedrock Foundation Models in your AWS account.
Download Prerequisite Files:
Download the book.txt file from the provided GitHub repository.

2. Create an S3 Bucket and Upload Files (Amazon S3)
Create Bucket:
Open the S3 Console, create a bucket, and keep settings default.
Upload Files:
Upload the book.txt file to the newly created bucket.

3. Create Amazon Bedrock Knowledge Bases (Amazon Bedrock)
Open Bedrock Console:
Navigate to the Amazon Bedrock Console.
Create Knowledge Base:
Name your Knowledge Base and provide a description.
Keep other settings default and proceed.

4. Configure Data Source in Bedrock
Link S3 Bucket:
Specify the S3 bucket as the data source for the Knowledge Base.
Choose Embeddings Model:
Select Titan Text Embeddings V2 for vectorizing your data.
Sync Data:
Sync the data source to generate vectors for efficient retrieval.

5. Test the Knowledge Base
Select Model:
Choose a pre-selected model like Claude 3 Sonnet v1 for queries.
Run Query:
Enter a query (e.g., "What steps should I follow before making the decision to become self-employed?").
Review the response and verify source details for accuracy.

6. Clean Up Resources
Delete Knowledge Bases:
Navigate to Bedrock Console, select Knowledge Base, and delete associated data sources and Knowledge Bases.
Delete Amazon OpenSearch Collections:
Remove vector store collections in the OpenSearch Console.
Delete S3 Bucket:
Empty and delete the S3 bucket created during the setup.
