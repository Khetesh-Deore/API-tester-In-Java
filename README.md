# API Tester

A modern JavaFX-based API testing tool that provides a user-friendly interface for testing REST APIs. This application allows you to send HTTP requests, view responses, and maintain a history of your API calls.

![API Tester Screenshot](screenshot.png)

## Features

- **HTTP Methods Support**: GET, POST, PUT, DELETE
- **Response Formatting**: Plain Text, JSON, and XML with syntax highlighting
- **Request History**: Track and view past API calls
- **Modern UI**: Clean and intuitive interface with dark/light themes
- **Performance Metrics**: Response time and size tracking
- **Error Handling**: Clear error messages and status indicators
- **Keyboard Shortcuts**: Quick access to common actions

## Prerequisites

- Java 17 or later
- Maven 3.6 or later

## Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd api-tester
```

2. Build the project:
```bash
mvn clean package
```

3. Run the application:
```bash
mvn javafx:run
```

Or run the packaged JAR:
```bash
java -jar target/api-tester-1.0-SNAPSHOT.jar
```

## Usage

### Making API Requests

1. Select the HTTP method from the dropdown menu (GET, POST, PUT, DELETE)
2. Enter the API endpoint URL
3. For POST/PUT requests, enter the request body in JSON format
4. Click "Send Request" or press Ctrl+Enter
5. View the formatted response in the center panel

### Response Information

- **Status Code**: Color-coded success/error indicators
- **Response Time**: Time taken for the request to complete
- **Response Size**: Size of the response in bytes/KB/MB
- **Format Options**: Switch between Plain Text, JSON, and XML views

### Request History

- View all past requests in the history panel
- Each entry shows method, URL, and status code
- Click on history entries to view details

### Keyboard Shortcuts

- `Ctrl + Enter`: Send request
- `Ctrl + S`: Save current request
- `Ctrl + H`: Toggle history panel
- `Ctrl + R`: Clear response

## Project Structure

```
api-tester/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── apitester/
│       │           ├── ApiTester.java
│       │           └── RequestEntry.java
│       └── resources/
│           └── styles.css
├── pom.xml
└── README.md
```

## Dependencies

- JavaFX 17.0.2
- org.json for JSON processing
- Java 17 HTTP Client

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. Here's how you can contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with JavaFX for modern UI
- Inspired by popular API testing tools like Postman
- Uses Java's built-in HTTP client for reliable requests
