# AI Email Writer - Backend

This is the backend for the AI-powered Email Reply Generator. It is built with Spring Boot and integrates with Google's Gemini AI model to generate email replies based on given content and tone. Additionally, it leverages AWS S3 for storage and AWS Elastic Beanstalk for deployment.

## Features
- REST API to generate AI-powered email replies
- Integration with Google's Gemini AI API
- AWS S3 for storage
- Deployment on AWS Elastic Beanstalk
- CORS enabled for frontend integration

## Technologies Used
- Java 21
- Spring Boot 3.4.3
- WebFlux for non-blocking API requests
- Lombok for reduced boilerplate code
- Maven for dependency management
- AWS S3 for cloud storage
- AWS Elastic Beanstalk for hosting

## Installation

### Prerequisites
- Java 21 installed
- Maven installed
- Google Cloud API Key for Gemini API
- AWS credentials configured for S3 access

## Running Path
To use this project, access the frontend via:
   ```
   http://ai-email-writer-front.s3-website.eu-north-1.amazonaws.com/
   ```

## Related Projects
To use this backend effectively, you will need the following related projects:

### Frontend (React-based UI)
- Repository: [AI Email Writer Frontend](https://github.com/JohnUfo/ai-email-writer-front.git)
- Provides a user-friendly interface for generating AI-powered email replies.

### Chrome Extension
- Repository: [AI Email Writer Extension](https://github.com/JohnUfo/ai-email-writer-extension.git)
- Allows users to generate email replies directly from their Gmail inbox using the AI model.

Ensure both the frontend and the extension are properly set up to use this backend API.

