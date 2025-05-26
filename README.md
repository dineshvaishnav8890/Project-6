# 🌐 Scalable Static Website Deployment using S3 + Cloudflare + GitHub Actions

This project demonstrates how to host and auto-deploy a static website using **AWS S3** (Free Tier), **Cloudflare** for global CDN and HTTPS, and **GitHub Actions** for CI/CD deployment.

---

## 🚀 Project Objective

To automate the deployment of a static HTML site to an S3 bucket, serve it via a custom domain through Cloudflare with HTTPS, and ensure scalability and speed using caching and versioning.

---

## 🛠️ Tech Stack

- **AWS S3** — Static site hosting
- **Cloudflare** — DNS, CDN, SSL
- **GitHub Actions** — CI/CD automation
- **HTML/CSS** — Static content
- **Bash** — CLI scripting

---

## 📋 Mini Guide

### ✅ 1. Create and Push Static Site to GitHub
```bash
echo '<h1>Hello from S3!</h1>' > index.html
git init
git remote add origin https://github.com/your-username/static-site.git
git add . && git commit -m "Initial commit"
git push -u origin main








✅ 2. AWS S3 Setup
Create a bucket with public access and enable static website hosting.

Add a bucket policy to allow public read access.

Enable bucket versioning.

✅ 3. GitHub Actions for CI/CD
.github/workflows/deploy.yml:


✅ 4. Cloudflare Configuration
Add your domain to Cloudflare and change nameservers.

Create a CNAME to point to the S3 website URL.

Enable SSL/TLS and turn on Always Use HTTPS.

Configure caching rules for static assets.






🌍 Live Site
🔗 http://my-static-site-labs.s3-website.eu-north-1.amazonaws.com







✅ Deliverables
 GitHub Actions CI/CD Workflow

 S3 + Cloudflare Integration

 Live HTTPS Static Website

 Cache Settings + Versioning

 Deployment Documentation (this README)










