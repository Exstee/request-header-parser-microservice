# Request Header Parser Microservice

[![Node.js CI](https://img.shields.io/badge/node.js-18.x-green)](https://nodejs.org/)
[![freeCodeCamp](https://img.shields.io/badge/freeCodeCamp-Project-blue)](https://www.freecodecamp.org/learn/back-end-development-and-apis/back-end-development-and-apis-projects/request-header-parser-microservice)
[![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](#license)

This is my implementation of the **Request Header Parser Microservice** for the freeCodeCamp Back End Development and APIs certification. It’s based on the official [boilerplate project](https://github.com/freeCodeCamp/boilerplate-project-headerparser).

---

## 🚀 Live Demo

You can try the live project here:  
👉 **[Live App on Replit](https://015bc6d1-8c74-4450-addc-8714c8318d8c-00-1f706x7gdlsh8.janeway.replit.dev/)**  

---

## 📦 Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Exstee/request-header-parser-microservice.git
   cd request-header-parser-microservice
````

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the server:

   ```bash
   npm start
   ```

   The app will listen on the port defined in `process.env.PORT` or fallback to `3000`.

---

## 📡 API Endpoint

### `GET /api/whoami`

Returns a JSON object with:

* `ipaddress` — your IP address
* `language` — the `Accept-Language` header
* `software` — the `User-Agent` header

#### Example Request

```
GET https://your-app-url/api/whoami
```

#### Example Response

```json
{
  "ipaddress": "203.0.113.195",
  "language": "en-US,en;q=0.9",
  "software": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7)"
}
```

---

## 🧩 Project Notes

* This microservice is built to pass the freeCodeCamp test suite.
* Middleware used:

  * `dotenv` for environment configuration
  * `express` for server setup
  * `cors` for cross-origin requests
* Static files are served from `/public`.

---

## 📄 License

This project is licensed under the **MIT License**.
Built as part of the [freeCodeCamp Back End Development and APIs curriculum](https://www.freecodecamp.org/learn/).

`````