# Audio-To-Text_SpringAI
This repository contains an application that converts audio files into text using Spring AI and the OpenAI API. The project leverages modern AI tools to provide accurate and efficient audio-to-text transcription services.

Features

Converts audio files (e.g., MP3, WAV) into text.

Uses the OpenAI API for transcription.

Built using Spring Boot for backend services.

Easily configurable with your own OpenAI API key.

Support for multiple audio file formats.

Prerequisites

Before running the project, ensure you have the following:

Java (version 17 or higher)

Maven (for dependency management)

An OpenAI API key (sign up at OpenAI to obtain one)

Installation

Clone the repository:

git clone https://github.com/yourusername/audio-to-text-converter.git
cd audio-to-text-converter

Configure your OpenAI API key:

Create a application.properties file in the src/main/resources directory.

Add the following configuration:

openai.api.key=your_openai_api_key_here
spring.application.name=AudioToTextConverter
server.port=8080

Build the project:

mvn clean install

Run the application:

mvn spring-boot:run

Usage

Upload Audio File:

Navigate to http://localhost:8080.

Use the provided web interface to upload your audio file.

Get Transcription:

After uploading, the application will process the file and return the transcribed text.

API Usage:

You can also use the REST API endpoint to upload files programmatically:

POST http://localhost:8080/api/transcribe
Content-Type: multipart/form-data
File: [audio_file]

The API will return the transcription as a JSON response.

Dependencies

This project uses the following dependencies:

Spring Boot: For creating the backend API.

OpenAI SDK: For integrating the OpenAI API.

Apache Commons FileUpload: For handling file uploads.

SLF4J: For logging.

Future Enhancements

Add support for real-time audio transcription.

Enhance error handling and validation.

Add multi-language support for transcription.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Contributing

Contributions are welcome! Please follow these steps:

Fork the repository.

Create a feature branch (git checkout -b feature-name).

Commit your changes (git commit -m "Added feature").

Push to the branch (git push origin feature-name).

Create a pull request.

Contact

For any questions or suggestions, feel free to contact:

Your Name: kalairoxan7973@gmail.com

GitHub: kalairoxan
