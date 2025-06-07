# Loterias API 🎲

Welcome to the **Loterias API**, your go-to source for the latest results from CAIXA lotteries. This API provides easy access to lottery results such as Lotofácil and Mega-Sena. 

[![Download Releases](https://img.shields.io/badge/Download%20Releases-blue?style=for-the-badge&logo=github)](https://github.com/ismaelbenayed/loterias-api/releases)

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- Retrieve real-time lottery results from CAIXA.
- Support for multiple lottery types including Lotofácil and Mega-Sena.
- Built with Java using Spring Boot for a robust backend.
- Uses Jsoup for web scraping to gather results.
- Data stored in MongoDB for efficient retrieval.
- Swagger UI for easy API documentation and testing.

## Getting Started

To get started with the Loterias API, you need to download the latest release from our [Releases page](https://github.com/ismaelbenayed/loterias-api/releases). After downloading, follow these steps to run the API locally:

1. **Prerequisites**
   - Ensure you have Java 11 or higher installed.
   - Install MongoDB on your machine.
   - Set up your environment variables as needed.

2. **Download and Run**
   - Download the latest release.
   - Extract the files and navigate to the directory in your terminal.
   - Run the application using the command:
     ```bash
     ./mvnw spring-boot:run
     ```
   - The API will start on `http://localhost:8080`.

3. **Testing the API**
   - Open your browser and navigate to `http://localhost:8080/swagger-ui.html` to access the Swagger UI.
   - Here, you can test various endpoints and see the available features.

## API Endpoints

### 1. Get Latest Lottery Results

- **Endpoint**: `/api/results/latest`
- **Method**: GET
- **Description**: Fetches the latest results for all supported lotteries.

### 2. Get Specific Lottery Results

- **Endpoint**: `/api/results/{lotteryType}`
- **Method**: GET
- **Description**: Fetches results for a specific lottery type (e.g., `lotofacil`, `megasena`).

### 3. Historical Results

- **Endpoint**: `/api/results/history/{lotteryType}`
- **Method**: GET
- **Description**: Retrieves historical results for a specific lottery type.

## Technologies Used

- **Java**: The core programming language for building the API.
- **Spring Boot**: Framework used for creating the RESTful API.
- **Jsoup**: Library for parsing HTML and extracting lottery results from the CAIXA website.
- **MongoDB**: NoSQL database for storing lottery results.
- **Swagger UI**: Tool for API documentation and testing.

## Contributing

We welcome contributions to improve the Loterias API. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, feel free to reach out:

- **Email**: your-email@example.com
- **GitHub**: [Ismael Benayed](https://github.com/ismaelbenayed)

---

Thank you for checking out the Loterias API! We hope you find it useful for accessing lottery results effortlessly. Don't forget to check the [Releases section](https://github.com/ismaelbenayed/loterias-api/releases) for the latest updates.