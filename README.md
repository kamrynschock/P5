# CSCE 412: Project 5 - CI/CD Web Deployment

## Overview
This repository contains the source code for my static website hosted on AWS S3. It is connected to an **AWS CodePipeline** to demonstrate a full CI/CD (Continuous Integration/Continuous Delivery) workflow.

## Project Objectives
* **Automation:** Any changes pushed to this GitHub repository automatically trigger the AWS CodePipeline.
* **Deployment:** The pipeline pulls the latest code and deploys it to my S3 bucket (`csce412kamrynschock.me`).
* **Security:** Access is restricted to the custom domain, ensuring direct S3 endpoints are inaccessible per project requirements.

## How to Update the Website
1.  Clone this repository to your local machine.
2.  Make changes to `index.html` or other assets.
3.  Commit the changes: 
    ```bash
    git add .
    git commit -m "Update website content"
    ```
4.  Push to GitHub:
    ```bash
    git push origin main
    ```
5.  Wait ~60 seconds for the **AWS CodePipeline** to detect the change and update the live site.

## Website Link
[http://csce412kamrynschock.me](http://csce412kamrynschock.me)