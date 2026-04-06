# API Testing Automation

Professional API testing suite with **Postman**, **Newman**, and automated HTML reporting.

This repository contains a ready-to-run Postman collection with environment configuration and automated test execution using **Newman**.

---

## 🚀 Project Overview

This project helps you:

- Organize and maintain API tests in a structured Postman collection  
- Run tests automatically using **Newman**  
- Generate human-friendly HTML reports for CI/CD feedback  
- Execute test suites locally or in pipelines

---

## 📁 Repository Structure

.
├── collections/  
│   └── API-Collection.postman_collection.json  
├── environments/  
│   └── production.postman_environment.json  
├── results/ (HTML reports after test execution)  
├── package.json  
├── .gitignore  
├── TESTING.md  
└── CONTRIBUTING.md  

---

## 🛠️ Requirements

- Node.js & npm  
- Newman & Newman HTML Reporter (installed as dev dependencies)

---

## 🧪 Running Tests Locally

Install dependencies:

```
npm install
```

Run all tests:

```
npm test
```

Run tests with detailed output:

```
npm run test:verbose
```

Run specific suites (e.g., Products or Authentication):

```
npm run test:products
npm run test:auth
```

Clear previous results:

```
npm run clean
```

After running, the HTML report will be in the `results/` folder.

---

## 📊 Reports

- CLI output shows pass/fail status  
- HTML report includes detailed request/response logs  

---

## 🤝 Contributing

To add new API tests:

1. Open the Postman collection (`collections/API-Collection.postman_collection.json`)  
2. Add your requests and tests  
3. Export the updated collection  
4. Run tests locally to ensure all checks pass  
5. Create a pull request  

See **CONTRIBUTING.md** for more details.

---

## 📝 Testing Guide

This suite includes tests such as:

- ✅ Status code validation  
- 🔍 Response structure & field validation  
- 📊 Data value assertions  
- ⚡ Performance checks  
- 🧯 Error handling tests  

Refer to **TESTING.md** for more details.

---

## 💡 CI/CD Integration

You can connect this suite to a pipeline (GitHub Actions, GitLab CI, Jenkins, etc.) to run API tests on push or merge events, and fail the build if tests fail.

---

## 📌 License

Published under the **ISC License**.

