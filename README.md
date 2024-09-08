# Text-to-Speech Converter Web Application 🎙️🔊

## Overview

The Text-to-Speech Converter Web Application allows users to convert text input into MP3 audio files. Leveraging AWS services, this application uses AWS Polly for text-to-speech synthesis and AWS S3 for storing the resulting audio files. Users can input text, generate speech, and listen to the audio directly in their browser.

## Key Features 🌟

- **Text Input and Conversion:** Users enter text into a textarea and click "Convert to MP3" to generate speech. ✍️➡️🔊
- **Speech Synthesis:** AWS Lambda processes the request, synthesizes speech using AWS Polly, and stores the MP3 file in AWS S3. ☁️🔄
- **Audio Playback:** Users can play the generated MP3 file directly within their browser using an HTML audio player. 🎵
- **Error Handling:** Displays user-friendly error messages for empty inputs or issues with audio generation. ❗

## Technical Details 🛠️

### Frontend

- **Technologies:** HTML, CSS, JavaScript
- **Features:**
  - Responsive design with a clean and modern interface. 📱💻
  - Input field and button for text submission. 📥🔘
  - Audio player for playback of the generated MP3 file. 🎧
  - Error messages for feedback. 🚨

### Backend

- **AWS Lambda:** Processes the text-to-speech conversion request. ⚙️
- **AWS Polly:** Converts text into speech in MP3 format. 🗣️🎤
- **AWS S3:** Stores the generated MP3 file. 📂

### API Integration

- **AWS API Gateway:** Exposes an endpoint for the frontend to communicate with the Lambda function. 🌐
- **CORS Configuration:** Allows cross-origin requests to enable communication between the web application and API. 🔄

### Security and Configuration

- **CORS Settings:** Configured on the S3 bucket to allow access from the web application. 🔒
- **Permissions:** Properly set up for Lambda function and S3 bucket to ensure secure operations. 🔑

## Usage 🚀

1. **Navigate to the Web Application:**
   - Visit the web page hosting the application. 🌍

2. **Convert Text to Speech:**
   - Enter text in the provided input field.
   - Click the "Convert to MP3" button to initiate the conversion. 🔄

3. **Play the Audio:**
   - Once the MP3 file is generated, it will be available for playback directly in the embedded audio player. 🎵

## Future Enhancements 🚀

- Support for additional voices and languages in AWS Polly. 🌍🗣️
- User authentication for premium features. 🔐
- Text formatting options and saving favorite text-to-speech conversions. 💾

## Getting Started 🏁

To set up and deploy this project, follow these steps:

1. **Set up AWS Services:**
   - Configure AWS Polly for text-to-speech synthesis.
   - Create an S3 bucket for storing audio files.
   - Deploy AWS Lambda function and configure API Gateway.

2. **Deploy Frontend:**
   - Host the `index.html` file on a web server or an S3 bucket configured for static website hosting.

3. **Update API Endpoint:**
   - Ensure that the API Gateway endpoint is correctly referenced in the frontend JavaScript code.

### Website Preview
![צילום מסך 2024-09-08 140533](https://github.com/user-attachments/assets/789527a3-3ec5-4504-8cd4-a9bb1e14934c)

![צילום מסך 2024-09-08 142518](https://github.com/user-attachments/assets/613d1cb4-fee0-4a9a-baab-58f459b19c1a)
