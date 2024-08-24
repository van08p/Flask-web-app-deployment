# Azure web app deployment

This project demonstrates how to deploy a simple Flask/FastAPI application to Azure Web Apps using GitHub Actions for CI/CD.

## Prerequisites

- Azure account
- GitHub account

## 1. Create a Flask application

- Create a simple Flask application with a single endpoint that returns "Hello, Azure Web Apps!" when accessed.
- Install the required packages using pip. (pip install Flask)
- Create a `requirements.txt` file with the required packages. (Flask)

## 2. Create a GitHub repository

- Create GitHub repository
- Add requirement.txt and app.py to GitHub repository

## 3. Set up Azure web app

- Login to Azure
- Search for "App services" and click "Create"
- Fill required details
- Click "Review + Create" and then "Create"

## 4. Configure GitHub Actions for CI/CD

- In your repository click "Actions" and select "set up a workflow yourself"
- Create a configuration file as `main.yml`
- Set up Azure Publish Profile
  1. In azure portal, go to your Web App and click "Download publish profile"
  2. Navigate to your GitHub repository
  3. Go to "Settings" > "Secrets and variables" > "Actions"
  4. Add a new secret with the name "AZURE_PUBLISH_PROFILE" and paste the contents of publish profile and save it
- Configure GitHub Actions workflow

  ![Screenshot (142)](https://github.com/user-attachments/assets/b572c3a0-f241-4202-ad16-61ccb1799a1f)
  

## 5. Deploy the Application

- Push a commit to your main branch 
- GitHub Actions will automatically trigger the workflow and deploy the application to Azure Web Apps.
- Verify Deployment by visiting URL of your web abb.

  ![azure1](https://github.com/user-attachments/assets/67ae82ca-2c89-47bc-9ad2-879f7622a2f5)

  

