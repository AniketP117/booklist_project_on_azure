
# 🌍 PlacePicker Project

A visually appealing and responsive **PlacePicker Application** built with **React**, **Vite**, and **Tailwind CSS**. 
It enables users to create a personal collection of places they would like to visit or have visited. 
The application is deployed using **AWS S3** and **CloudFront** with the **AWS CLI**.

---

## 🚀 Features

- 🌏 Select and store places of interest
- 📸 Visually engaging interface with images of various destinations
- ⚡ Fast and optimized with Vite
- ☁️ Hosted on AWS with automatic deployment using AWS CLI

---

## 🛠️ Tech Stack

| Tech               | Purpose                    |
|--------------------|-----------------------------|
| **React**          | Frontend UI library         |
| **Vite**           | Bundler & dev server        |
| **Tailwind CSS**   | Styling                     |
| **AWS S3**         | Static hosting              |
| **CloudFront**     | CDN for faster access       |

---

## 🧑‍💻 Uploading to GitHub

1. **Initialize a Git Repository:**
   ```bash
   git init
   ```

2. **Add Remote Repository:**
   ```bash
   git remote add origin https://github.com/your-username/repo-name.git
   ```

3. **Add Files to Git:**
   ```bash
   git add .
   ```

4. **Commit Your Changes:**
   ```bash
   git commit -m "Initial commit for PlacePicker Project"
   ```

5. **Push to GitHub:**
   ```bash
   git push -u origin main
   ```

---

## ☁️ Deploying on AWS S3

1. **Configure AWS CLI:**
   ```bash
   aws configure
   ```

2. **Build the Project:**
   ```bash
   npm run build
   ```

3. **Upload Build Files to S3:**
   ```bash
   aws s3 cp ./dist s3://your-bucket-name --recursive
   ```

4. **Configure Bucket for Static Website Hosting:**
   ```bash
   aws s3 website s3://your-bucket-name/ --index-document index.html --error-document index.html
   ```

5. **Invalidate CloudFront Cache (if needed):**
   ```bash
   aws cloudfront create-invalidation --distribution-id YOUR_DISTRIBUTION_ID --paths "/*"
   ```

---

## 🌐 Live Demo
https://booklist-project-2025.s3.us-east-1.amazonaws.com/index.html
