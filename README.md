
# Static Website Hosting on AWS with S3, CloudFront, Route 53, and ACM

This project demonstrates how to host a secure and highly available static website on **Amazon Web Services (AWS)** using the following services:  

- **Amazon S3** – For storing and serving static website files.  
- **Amazon CloudFront** – As a global CDN to deliver content with low latency.  
- **AWS Certificate Manager (ACM)** – To provision and manage SSL/TLS certificates for HTTPS.  
- **Amazon Route 53** – For DNS routing and domain management.  

---

##  Project Overview

The goal of this project is to showcase how to host a **production-ready static website** on AWS with:  
- Custom domain integration.  
- End-to-end encryption via HTTPS.  
- Global distribution and caching for performance optimization.  
- High availability and scalability using AWS-managed services.  

---

## 🛠️ Architecture

**Workflow:**
1. Static website files are uploaded to an **S3 bucket** configured for static website hosting.  
2. **CloudFront distribution** is set up to cache and deliver the content globally.  
3. **ACM** provides SSL certificates to enforce HTTPS.  
4. **Route 53** is used to route traffic from a custom domain to the CloudFront distribution.  

---

 **Architecture Diagram:**
[Architecture Diagram](./Static-hosting-architecture.png)


📂 Project Structure
.
├── index.html
├── styles.css
├── script.js
├── images
└── README.md

---

## Security Considerations

- SSL/TLS enabled through AWS Certificate Manager.

- CloudFront is configured to redirect all traffic to HTTPS.

- S3 bucket access restricted to CloudFront (Origin Access Control/Identity).

  ---

## Key Benefits

- Scalability: AWS-managed services scale with traffic.

- Performance: CloudFront ensures low latency with edge caching.

- Security: HTTPS with ACM-managed certificates.

- Reliability: Route 53 ensures highly available DNS resolution.

  

## Deployment Steps

- Upload website files to an S3 bucket.

- Create a CloudFront distribution pointing to the S3 bucket.

- Request a certificate via AWS Certificate Manager.

- Configure Route 53 to map your domain to the CloudFront distribution.

- Verify HTTPS by accessing your domain securely.

--- 

  ## 📚 Skills Learned
- S3 hosting & CloudFront caching.  
- SSL/TLS setup with ACM.  
- DNS management with Route 53.  
- Cost optimization for low-traffic websites.  

---

## 📌 Next Steps
- Add CI/CD pipeline for automatic deployment.  
- Integrate CloudWatch monitoring for performance.  

---

## Author

Prinston Sarfo

- Cloud/DevOps Enthusiast

- Passionate about AWS & scalable architectures

  ---

## License

This project is licensed under the MIT License – feel free to use, modify, and share.
