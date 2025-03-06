# AI Email Writer - Backend

This is the backend for the AI-powered Email Reply Generator. It is built with Spring Boot and integrates with Google's Gemini AI model to generate email replies based on given content and tone.

## Features
- REST API to generate AI-powered email replies
- Integration with Google's Gemini AI API
- CORS enabled for frontend integration

## Technologies Used
- Java 21
- Spring Boot 3.4.3
- WebFlux for non-blocking API requests
- Lombok for reduced boilerplate code
- Maven for dependency management

## Installation

### Prerequisites
- Java 21 installed
- Maven installed
- Google Cloud API Key for Gemini API

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/JohnUfo/ai-email-writer-extension.git
   cd ai-email-writer-extension
   ```
2. Configure your API key:
   - In the `application.properties` or `application.yml` file, set the following values:
     ```properties
     gemini.api.url=https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=
     gemini.api.key=YOUR_GEMINI_API_KEY
     ```
   - Replace `YOUR_GEMINI_API_KEY` with your actual API key (see [this guide](https://scribehow.com/shared/How_To_Create_An_API_Key_in_Google_Cloud__laekAQbTQVavJN4V-ZY0Gg)).
3. Build and run the application:
   ```sh
   mvn clean install
   mvn spring-boot:run
   ```
4. The API will be available at:
   ```sh
   http://localhost:8080/api/email/generate
   ```

## API Endpoint
### Generate AI Email Reply
- **Endpoint:** `POST /api/email/generate`
- **Request Body:**
  ```json
  {
    "emailContent": "Hello, can we reschedule our meeting?",
    "tone": "professional"
  }
  ```
- **Response:**
  ```json
  "Sure, let me know a convenient time for you."
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

