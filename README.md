# Google Calendar to Slack Notification with AWS Lambda

This project is designed to fetch events from a Google Calendar and push updates to a Slack channel at regular intervals using AWS Lambda. The entire workflow, including deployment, is automated using GitHub Actions.

## Features
- Fetches events from a shared Google Calendar.
- Posts calendar events to a Slack channel.
- Uses AWS Lambda to run the event fetching and posting process periodically.
- Automates deployment to AWS Lambda using GitHub Actions.

## Prerequisites

### 1. Google Calendar API
- You need to create a Google Cloud project and enable the **Google Calendar API**.
- Set up OAuth2.0 credentials for your project.
- Download the `credentials.json` file from Google Cloud Console and add it to your project.

### 2. AWS Lambda
- AWS Lambda function with necessary IAM permissions (e.g., `AWSLambdaBasicExecutionRole`).
- Set up AWS CLI or use your AWS account credentials for deployment.

### 3. Slack API
- Create a Slack App and add it to the desired workspace.
- Generate an OAuth Token for the app that has permission to post messages to channels (`chat:write` scope).

### 4. GitHub Repository
- Store the Lambda function code and related configuration in your GitHub repository.
- Set up GitHub Actions for CI/CD and deployment.
