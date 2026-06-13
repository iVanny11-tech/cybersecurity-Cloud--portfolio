# ☁️ AWS 2-Tier Web Application Project

This project shows how I built a **2-tier architecture** on **AWS** — a simple setup with:
- 🖥️ **Frontend (Web Server)** in a **Public Subnet**
- 🗄️ **Backend (Database)** in a **Private Subnet**

It’s a beginner-friendly AWS networking project that helped me understand how **VPCs**, **subnets**, and **security groups** work together.

---

## 🧱 Architecture Overview


✅ Public Subnet → Internet access for web traffic  
✅ Private Subnet → Hidden from the internet  
✅ Security Groups → Control who can access what  

---

## ⚙️ Tools & AWS Services Used

- **Amazon VPC** — to create my own private network  
- **Subnets** — divided into Public & Private  
- **Internet Gateway** — to connect the public subnet to the internet  
- **EC2 Instances** — for web server and database  
- **Security Groups** — to allow/deny traffic  
- *(Optional)* **NAT Gateway** — to let private subnet download updates  

---

## 🪜 Step-by-Step Summary

### 🧩 Step 1 — Create a VPC
Created a new **VPC** with the CIDR range `10.0.0.0/16`.

### 🌐 Step 2 — Create Subnets
- **Public Subnet:** `10.0.1.0/24` (for web server)
- **Private Subnet:** `10.0.2.0/24` (for database)

Enabled **Auto-assign Public IP** on the public subnet.

### 🚪 Step 3 — Internet Gateway
Attached an **Internet Gateway** to the VPC for external access.

### 🧭 Step 4 — Route Tables
- Public route table → route to Internet Gateway  
- Private route table → no direct internet route  

### 💻 Step 5 — Launch EC2 Instances
- Web Server (Frontend) → Public subnet  
- Database (Backend) → Private subnet  

Used **Amazon Linux 2** AMI (Free Tier eligible).

### 🔐 Step 6 — Configure Security Groups
- **Web SG:** allows HTTP (80) and SSH (22)  
- **DB SG:** allows MySQL (3306) only from Web SG  

### ⚡ Step 7 — Install Web Server
SSH’d into the web EC2 and ran:

```bash
sudo yum update -y
sudo yum install -y httpd
sudo systemctl start httpd
sudo systemctl enable httpd
echo "<h1>Hello from my AWS Web Server!</h1>" | sudo tee /var/www/html/index.html

✅ Public Subnet → Internet access for web traffic  
✅ Private Subnet → Hidden from the internet  
✅ Security Groups → Control who can access what  

---

## ⚙️ Tools & AWS Services Used

- **Amazon VPC** — to create my own private network  
- **Subnets** — divided into Public & Private  
- **Internet Gateway** — to connect the public subnet to the internet  
- **EC2 Instances** — for web server and database  
- **Security Groups** — to allow/deny traffic  
- *(Optional)* **NAT Gateway** — to let private subnet download updates  

---

## 🪜 Step-by-Step Summary

### 🧩 Step 1 — Create a VPC
Created a new **VPC** with the CIDR range `10.0.0.0/16`.

### 🌐 Step 2 — Create Subnets
- **Public Subnet:** `10.0.1.0/24` (for web server)
- **Private Subnet:** `10.0.2.0/24` (for database)

Enabled **Auto-assign Public IP** on the public subnet.

### 🚪 Step 3 — Internet Gateway
Attached an **Internet Gateway** to the VPC for external access.

### 🧭 Step 4 — Route Tables
- Public route table → route to Internet Gateway  
- Private route table → no direct internet route  

### 💻 Step 5 — Launch EC2 Instances
- Web Server (Frontend) → Public subnet  
- Database (Backend) → Private subnet  

Used **Amazon Linux 2** AMI (Free Tier eligible).

### 🔐 Step 6 — Configure Security Groups
- **Web SG:** allows HTTP (80) and SSH (22)  
- **DB SG:** allows MySQL (3306) only from Web SG  

### ⚡ Step 7 — Install Web Server
SSH’d into the web EC2 and ran:

```bash
sudo yum update -y
sudo yum install -y httpd
sudo systemctl start httpd
sudo systemctl enable httpd
echo "<h1>Hello from my AWS Web Server!</h1>" | sudo tee /var/www/html/index.html






✅ Public Subnet → Internet access for web traffic  
✅ Private Subnet → Hidden from the internet  
✅ Security Groups → Control who can access what  

---

## ⚙️ Tools & AWS Services Used

- **Amazon VPC** — to create my own private network  
- **Subnets** — divided into Public & Private  
- **Internet Gateway** — to connect the public subnet to the internet  
- **EC2 Instances** — for web server and database  
- **Security Groups** — to allow/deny traffic  
- *(Optional)* **NAT Gateway** — to let private subnet download updates  

---

## 🪜 Step-by-Step Summary

### 🧩 Step 1 — Create a VPC
Created a new **VPC** with the CIDR range `10.0.0.0/16`.

### 🌐 Step 2 — Create Subnets
- **Public Subnet:** `10.0.1.0/24` (for web server)
- **Private Subnet:** `10.0.2.0/24` (for database)

Enabled **Auto-assign Public IP** on the public subnet.

### 🚪 Step 3 — Internet Gateway
Attached an **Internet Gateway** to the VPC for external access.

### 🧭 Step 4 — Route Tables
- Public route table → route to Internet Gateway  
- Private route table → no direct internet route  

### 💻 Step 5 — Launch EC2 Instances
- Web Server (Frontend) → Public subnet  
- Database (Backend) → Private subnet  

Used **Amazon Linux 2** AMI (Free Tier eligible).

### 🔐 Step 6 — Configure Security Groups
- **Web SG:** allows HTTP (80) and SSH (22)  
- **DB SG:** allows MySQL (3306) only from Web SG  

### ⚡ Step 7 — Install Web Server
SSH’d into the web EC2 and ran:

```bash
sudo yum update -y
sudo yum install -y httpd
sudo systemctl start httpd
sudo systemctl enable httpd
echo "<h1>Hello from my AWS Web Server!</h1>" | sudo tee /var/www/html/index.html


Name: [Ivan Yamoah Boakye]
Date: [Nov, 2025]
LinkedIn: [www.linkedin.com/in/ivan-yamoah-boakye-70594523a]
