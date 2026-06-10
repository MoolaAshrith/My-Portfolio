# My-Portfolio
# Automated CI/CD Portfolio Deployment on AWS

## Overview

This project demonstrates an automated CI/CD pipeline for deploying a static portfolio website using GitHub Actions and AWS services.

Whenever code is pushed to GitHub, GitHub Actions automatically deploys the latest website files to an AWS S3 bucket and invalidates the CloudFront cache, ensuring users always see the latest version.

---

## Architecture

Developer
↓
GitHub Repository
↓
GitHub Actions
↓
AWS S3 Bucket
↓
CloudFront CDN
↓
Live Portfolio Website

---

## Technologies Used

- AWS S3
- AWS CloudFront
- AWS IAM
- GitHub
- GitHub Actions
- AWS CLI
- HTML
- CSS

---

## Features

- Automated CI/CD deployment
- Static website hosting on AWS S3
- Global content delivery using CloudFront
- HTTPS enabled
- Automatic CloudFront cache invalidation
- Secure AWS authentication using GitHub Secrets

---

## Project Structure

```text
MY-PORTFOLIO/
│
├── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── images/
│   └── Myresume2.pdf
│
└── .github/
    └── workflows/
        └── deploy.yml
