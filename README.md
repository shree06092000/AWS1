# AWS-Project-1
Deploying A Multi-Tier Website Using AWS EC2

☁️ High Availability Web Application on AWS (EC2 + RDS + Auto Scaling)

📖 Project Overview

This project demonstrates how to migrate a traditional web application to the Amazon Web Services (AWS) cloud with a focus on scalability, availability, and security. By leveraging Amazon EC2 for compute, Amazon RDS for database management, and Auto Scaling for elasticity, the solution ensures that Company ABC’s PHP-based website and MySQL database can handle traffic spikes seamlessly while maintaining high availability.

🎯 Problem Statement

    Company ABC currently hosts:
    
          A PHP-based website
          
          A MySQL database
          
    The company wants to move its product to AWS and achieve high availability by enabling Auto Scaling on the website infrastructure.

🛠️ Solution Approach
    The migration was implemented through the following steps:
    
    Launch EC2 Instances
        
        Deployed PHP-based website on Amazon EC2.
        
        Configured security groups for controlled access.
    
    Enable Auto Scaling
    
        Configured Auto Scaling with a minimum of 2 EC2 instances.
        
        Ensured elasticity to handle traffic spikes.
    
    Create Amazon RDS Instance
    
        Provisioned a managed MySQL database using Amazon RDS.
        
        Database name: intel
        
        Table name: data
        
        Database password: intel123
    
    Application Configuration
    
        Updated website hostname to point to the RDS instance.
        
        Allowed traffic from EC2 to RDS securely.
        
        Configured EC2 instances to accept all incoming traffic for web access.

🔒 Security Considerations
        Security Groups configured to allow only necessary traffic.
        
        IAM Roles & Policies applied for least-privilege access.
        
        RDS used for managed database service with automated backups.
        
        HTTPS recommended for secure communication.

📈 Key Features
        Elastic Compute: EC2 instances scale automatically based on demand.
        
        High Availability: Minimum of 2 instances running at all times.
        
        Managed Database: Amazon RDS ensures reliability and automated maintenance.
        
        Seamless Integration: Website connected securely to RDS backend.

🚀 Future Enhancements
        Add Elastic Load Balancer (ELB) for distributing traffic across EC2 instances.
        
        Implement CloudWatch monitoring for proactive alerts.
        
        Enable Multi-AZ deployment for RDS to improve fault tolerance.
        
        Integrate CI/CD pipeline for automated deployments.

📌 Impact
This project showcases how cloud-native architecture can transform a traditional web application into a highly available, scalable, and secure solution. It highlights best practices in AWS infrastructure design and demonstrates practical skills in EC2, RDS, and Auto Scaling.
