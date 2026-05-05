AWS Auto Scaling & Load Balancer Deployment (Multi-AZ)

 📌 Overview
Designed and deployed a highly available and scalable web infrastructure on AWS using Auto Scaling and Application Load Balancer (ALB) across multiple Availability Zones.

🏗️ Architecture
User → Application Load Balancer → Auto Scaling Group → EC2 Instances → VPC

⚙️ Key Implementation

- Built custom VPC (10.0.0.0/16) with public subnets across multiple AZs  
- Configured Internet Gateway and route tables for public access  
- Deployed Application Load Balancer (ALB) across Multi-AZ  
- Created Target Group with HTTP health checks  
- Implemented Launch Template with automated user-data bootstrap (Apache + Instance ID display)  
- Configured Auto Scaling Group with CPU Target Tracking (50%)  

 🧪 Validation & Results

- Simulated CPU load using stress-ng  
- Verified automatic scale-out when CPU > 50%  
- Confirmed automatic scale-in when load reduced  
- Observed dynamic traffic distribution across healthy instances  

🚀 Infrastructure Capabilities

- High Availability (Multi-AZ design)  
- Elastic scalability under real load conditions  
- Secure security group segmentation (ALB → EC2 only)  
- Automated provisioning via Launch Templates  
- Production-style scaling policies and monitoring  

 📸 Screenshots

*(We will add screenshots next step)*

🎯 Outcome

Successfully built a resilient, scalable AWS infrastructure aligned with cloud engineering best practices.
