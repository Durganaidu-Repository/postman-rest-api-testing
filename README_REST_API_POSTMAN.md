
# REST API Testing Project using Postman

## 📌 Project Title
REST API Testing & Automation using Postman

## 📖 Project Overview
This project demonstrates REST API testing skills using **Postman**. It covers manual API testing, validations, environment variables, collections, and basic automation using JavaScript test scripts.  
The project is designed to showcase **API testing knowledge for fresher QA / Data / Backend roles**.

## 🛠 Tools & Technologies
- Postman
- REST APIs
- HTTP Methods (GET, POST, PUT, DELETE)
- JSON
- JavaScript (Postman Tests)
- Newman (optional)

## 📂 APIs Used
Public dummy API:
- https://reqres.in

## 📁 Project Structure
```
postman-rest-api-project/
│── README.md
│── collections/
│   └── ReqRes_API_Collection.json
│── environments/
│   └── ReqRes_Environment.json
│── screenshots/
│   └── test-results.png
```

## 🔹 API Test Scenarios Covered

### 1️⃣ GET Users
- Validate status code = 200
- Validate response time
- Validate user list is not empty

### 2️⃣ GET Single User
- Validate user ID
- Validate email format

### 3️⃣ POST Create User
- Validate status code = 201
- Validate name and job in response

### 4️⃣ PUT Update User
- Validate status code = 200
- Validate updated fields

### 5️⃣ DELETE User
- Validate status code = 204

## 🧪 Sample Postman Test Script
```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response time is less than 500ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(500);
});
```

## 🌍 Environment Variables
| Variable | Description |
|--------|------------|
| base_url | API base URL |
| user_id | Dynamic user ID |

## ▶️ How to Run the Project
1. Import the **Postman Collection**
2. Import the **Environment file**
3. Select the environment
4. Run the collection using **Collection Runner**
5. (Optional) Run using Newman CLI

## 📈 Key Learnings
- REST API fundamentals
- API testing life cycle
- Writing assertions in Postman
- Using environment & global variables
- Automating API tests

## 📌 Resume Description (Copy-Paste)
**REST API Testing Project (Postman):**
- Designed and executed API test cases using Postman for CRUD operations
- Validated response status codes, headers, response time, and JSON data
- Automated API validations using JavaScript test scripts
- Used environment variables for dynamic testing

## 👤 Author
**Durga Rao Thaddi**  
B.Sc Computers (2020)  
Aspiring Data Analyst / Backend Developer
