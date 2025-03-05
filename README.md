# aws-glue-minio-docker
docker-compose up --build -d

docker-compose down

# AWS Glue & minio S3 in local using docker
This guide explains how to set up AWS Glue with MinIO (a local S3-compatible storage) using Docker. This allows you to test AWS Glue jobs locally without needing an actual AWS S3 bucket.

## 🚀 Project Overview
This project demonstrates to locally run **AWS Glue** and **AWS S3**.  

## 🛠️ Tech Stack
- **AWS Services**: AWS S3, AWS Glue
- **ETL Tools**: AWS Glue, PySpark
- **File Storage**: S3 using Minio
- **Language**: Python

## Prerequisites
- **Docker & Docker Compose** installed on your machine

## 📌 Features
✅ Read data from AWS S3  
✅ Transformation using AWS Glue, PySpark  
✅ Loading data into AWS S3  

## 🚀 Deployment and Usage

1. Clone the repository:
    ``` bash
    git clone https://github.com/ItisVenkatesh/aws-glue-minio-docker.git
    cd aws-glue-minio-docker

2. Make sure that the Docker is running in your system.

3. Run docker-compose to start the containers:

    ``` bash
    docket-compose up --build -d

4. Configure MinIO S3 (Optional)

   - Open [http://localhost:9001](http://localhost:9001)
   - Login with:
     - **Username**: `minioadmin`
     - **Password**: `minioadmin`

5. Open Jupyter Notebook to work with AWS Glue
   - Open [http://localhost:8888](http://localhost:8888)
   - Try running the notebook glue_s3_access_local.ipynb or Explore by creating a new notebook

6. Run docker-compose to stop the containers:
   - Once done, to stop the containers,
   ``` bash
   docker-compose down

## Conclusion
You have now successfully set up AWS Glue to interact with MinIO S3 in a local Docker environment. This allows you to test Glue ETL jobs locally before deploying to AWS.

## License

This project is licensed under the MIT License - see the LICENSE file for details.