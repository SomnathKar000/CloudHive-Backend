# CloudHive-Backend

[![CloudHive](https://img.shields.io/badge/CloudHive-Backend-brightgreen)](https://github.com/SomnathKar000/CloudHive-Backend)
[![Frontend Repo](https://img.shields.io/badge/Frontend%20Repo-CloudHive-blue)](https://github.com/SomnathKar000/CloudHive)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-Cloud%20Hive-9cf)](https://cloud-hive.vercel.app/)

CloudHive is a web application that allows users to securely upload and manage files in the cloud. This repository contains the backend code for the CloudHive project. It is built using Node.js, Express, AWS S3, PostgreSQL, Sequelize, JWT for authentication, and bcryptjs for password hashing. Express-validator is used for request validation.

## Features

- **File Uploads:** Utilizes AWS S3 for secure file uploads through pre-signed URLs.

- **Database:** Stores user data and file keys in a PostgreSQL database.

- **ORM:** Interacts with the SQL database using Sequelize, a powerful ORM.

- **Authentication:** Implements JWT for user authentication, ensuring data security.

- **Password Hashing:** Uses bcryptjs to securely hash user passwords.

- **Request Validation:** Utilizes express-validator to validate incoming requests.

## Getting Started

Follow these steps to set up the CloudHive-Backend locally:

1. **Clone the repository:**

   ```shell
   git clone https://github.com/your-username/CloudHive-Backend.git
   ```

2. **Install Dependencies:**

   ```shell
   cd CloudHive-Backend
   npm install
   ```

3. **Set Environment Variables:**

   - Create a `.env` file in the root directory and add the following variables:

   ```plaintext
   PORT=3000

   AWS_ACCESS_KEY_ID=your-aws-access-key
   AWS_SECRET_ACCESS_KEY=your-aws-secret-key
   AWS_REGION=your-aws-region
   AWS_S3_BUCKET_NAME=your-aws-bucket-name
   jwt_secret=your-secret-key-for-jwt
   db_name=your-database-name
   db_host=your-database-host
   db_user=your-database-username
   db_password=your-database-password
   ```

4. **Start the Server:**
   ```shell
   npm start
   ```

Your backend server should now be running at `http://localhost:3000`.

## Deployed Application

The CloudHive application is hosted on Vercel. You can access it [here](https://cloud-hive.vercel.app/).
