# Intellispend

**Intellispend** is a budgeting app designed to help users gain control of their finances. This app utilizes the Plaid API to retrieve and categorize expenses, making it easier for users to track their spending and make informed financial decisions.

## Table of Contents

- [Intellispend](#intellispend)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Installation](#installation)
    - [Client](#client)
    - [Server](#server)
  - [Usage](#usage)
  - [Security](#security)
  - [Configuration](#configuration)
  - [Contributing](#contributing)
  - [Contributors](#contributors)
  - [License](#license)

## Features

- Connects to Plaid to retrieve transaction data.
- Categorizes and analyzes expenses to generate a pie chart.
- Allows users to set budget limits for different expense categories.
- Provides a user-friendly dashboard to visualize financial data.
- Helps users make informed financial decisions.

## Installation

To get started with **Intellispend**, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/drPod/intellispend.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Intellispend
   ```

3. Install the required dependencies for the client and server components. Refer to the client and server sections below for specific installation instructions.

4. Configure your Plaid API credentials (see [Configuration](#configuration) for details).

5. Run both the client and server components.

**Intellispend** should now be running locally, with both the client and server components accessible in your web browser and server port, respectively.

### Client

The **Intellispend Client** is the frontend component responsible for the user interface. To set up the client, follow these steps:

1. Navigate to the client directory:

   ```bash
   cd client
   ```

2. Install the required dependencies using npm:

   ```bash
   npm install
   ```

3. Start the client application:

   ```bash
   npm run dev
   ```

The client application will be accessible in your web browser.

### Server

The **Intellispend Server** is the backend component responsible for handling data retrieval and processing. To set up the server, follow these steps:

1. Navigate to the server directory:

   ```bash
   cd server
   ```

2. Install the required dependencies using npm:

   ```bash
   npm install
   ```

3. Configure your Plaid API credentials in the server component (see [Configuration](#configuration) for details).

4. Start the server application:

   ```bash
   npx nodemon index.ts
   ```

The server will be accessible via a specified port (default is 3000).

4. Configure your Plaid API credentials (see [Configuration](#configuration) for details).

5. Run the application:

   ```bash
   npm run dev
   ```

**Intellispend** should now be running locally and accessible in your web browser.

## Usage

Upon running the application, users can perform the following actions:

1. **Connect to Plaid**: To get started, users need to connect their bank accounts using Plaid. This will allow the app to retrieve transaction data and analyze expenses.

2. **View Expenses**: Once connected, users can view their expenses, categorized into different spending categories.

3. **Set Budgets**: Users can set budget limits for each spending category. The app will help them track their spending against these budgets.

4. **Visualize Data**: The app generates a pie chart that displays the distribution of expenses in various categories, making it easy for users to see where their money is going.

5. **Make Informed Decisions**: With expense data and budgeting insights, users can make informed financial decisions to manage their money effectively.

## Security

**Intellispend** takes security seriously to ensure the safety and privacy of user data. Here are some of the security measures in place:

1. **Data Encryption**: All sensitive user data, including Plaid API credentials, is securely stored and transmitted using encryption protocols. This helps protect the confidentiality of user information.

2. **User Authentication**: User accounts are protected with robust authentication mechanisms. Passwords are securely hashed and salted to prevent unauthorized access.

3. **Authorization**: The app uses role-based access control to restrict access to sensitive functionality and data. Users are only allowed to perform actions and access data relevant to their role.

4. **Plaid API Security**: The connection to the Plaid API is established using secure and authenticated methods. Plaid provides its own security measures to protect financial data during data retrieval.

5. **Validation and Sanitization**: User inputs are validated and sanitized to prevent common security vulnerabilities such as SQL injection and cross-site scripting (XSS) attacks.

6. **Regular Security Audits**: The codebase undergoes regular security audits and vulnerability assessments to identify and address potential security issues.

7. **Updates and Patching**: The app is maintained and updated to stay current with security patches and best practices.

While **Intellispend** has been designed with security in mind, it's essential for users to follow best security practices, such as using strong and unique passwords and being cautious about sharing their data with third-party services.

If you discover any security vulnerabilities or have concerns related to security, please report them by opening a security issue on this repository or contacting the project maintainers directly. Your assistance in improving the security of the app is greatly appreciated.

## Configuration

To use **Intellispend**, you need to configure your Plaid API credentials. Follow these steps:

1. Visit the [Plaid Developer Portal](https://dashboard.plaid.com/signup) and create an account or log in if you already have one.

2. Create a new Plaid API application and obtain your API keys.

3. In the project directory, create a `.env` file and add the following configuration:

   ```env
    API_KEY="your-api-key"
    AUTH_DOMAIN="your-auth-domain"
    PROJECT_ID="your-project-id"
    STORAGE_BUCKET="your-storage-bucket"
    SENDER_ID="your-sender-id"
    APP_ID="your-app-id"
    MEASUREMENT_ID="your-measurement-id"
    PLAID_ID="your-plaid-id"
    SANDBOX_SECRET="your-sandbox-secret"
    COOKIE_SECRET="your-cookie-secret"
   ```

4. Replace `your-api-key`, `your-auth-domain`, `your-project-id`, `your-storage-bucket`, `your-sender-id`, `your-app-id`, `your-measurement-id`, `your-plaid-id`, `your-sandbox-secret`, and `your-cookie-secret` with your Plaid API credentials.

5. Save the `.env` file.

Now, your app is configured to use the Plaid API for transaction data retrieval.

## Contributing

We welcome contributions to **Intellispend**. If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix: `git checkout -b feature/your-feature-name`.
3. Make your changes and commit them: `git commit -m "Add a new feature"`.
4. Push your changes to your fork: `git push origin feature/your-feature-name`.
5. Create a pull request on the main repository's `main` branch.

Please ensure your code follows our coding standards and include tests for new features or bug fixes.

## Contributors

[Jeff Zhou](www.github.com/jeffsummer08), [Rohan Sarakinti](https://github.com/rohansarakinti)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Thank you for using **Intellispend**. We hope this app helps you gain better control of your finances. If you have any questions or encounter issues, please feel free to open an issue on this repository. Happy budgeting!