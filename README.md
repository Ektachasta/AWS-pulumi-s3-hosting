# 🌍 AWS S3 Static Website Hosting with Pulumi

🚀 Deploy a static website on **AWS S3** using **Pulumi** with a simple **YAML** configuration.

---
## ✅ Prerequisites
Before you begin, ensure you have the following installed:

🔹 **Pulumi CLI** → [Install Pulumi](https://www.pulumi.com/docs/install/)

🔹 **AWS CLI** → [Install AWS CLI](https://aws.amazon.com/cli/)

🔹 **Git** → [Install Git](https://git-scm.com/)

### 🔐 Configure AWS Credentials
```sh
aws configure
```
You'll be prompted to enter:
- 🔑 **AWS Access Key ID**
- 🔒 **AWS Secret Access Key**
- 🌎 **Default AWS Region** (e.g., `us-east-1`)

---
## ⚙️ Install & Set Up Pulumi
Download and install Pulumi:
```sh
curl -fsSL https://get.pulumi.com | sh
```
After installation, restart your terminal and verify:
```sh
pulumi version
```

---
## 🚀 Clone & Deploy the Infrastructure
```sh
git clone https://github.com/Ektachasta/AWS-pulumi-s3-hosting
cd AWS-pulumi-s3-hosting
pulumi login
pulumi stack init dev
pulumi up
```
🎉 **Once deployed, Pulumi will return the S3 website URL!**

---
## 🌐 Access Your Website
Find your website URL using:
```sh
pulumi stack output websiteUrl
```

---
## 📌 Additional Information
- 🌟 **Static Website Hosting** → Enables S3 static website hosting for easy public access.
- 🔄 **Pulumi State Management** → Stores stack states remotely for seamless updates & rollbacks.
- 🔓 **Bucket Policy & Permissions** → Ensure the S3 bucket has public read access if needed.

---
## 🗑️ Cleanup (Optional)
To remove all AWS resources created by Pulumi:
```sh
pulumi destroy --yes
```

🚀 **Happy Coding & Cloud Deployment!** 🎉
