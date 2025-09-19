## 🧪 E-Commerce API Testing with Postman – Swagger Petstore
This project demonstrates manual API testing of the Swagger Petstore sample APIs using Postman.
It covers User, Pet, and Order APIs with essential smoke tests, negative cases, and a traceability matrix (RTM).

## 📌 Project Overview
- Objective: Validate Swagger Petstore APIs (User, Pet, Order modules).
- Scope: Perform CRUD operations, authentication checks, and input validation.
- Tools Used:
    - Postman : for API execution.
    - JSON collections : for one-click execution.
     -Excel Test Case and RTM : for test coverage.

## ✅ Included Smoke Tests
User APIs
- Create User
- Login User
- Get User by Username
- Logout User
  
## Pet APIs
- Add Pet
- Get Pet by ID
- Update Pet
- Delete Pet

## Order APIs
- Place Order
- Get Order by ID
- Delete Order

## 📝 Pre-written Tests
- Each request validates:
    - ✅ Status code (200, 4xx)
    - ✅ Response format (JSON)
    - ✅ Key fields exist (username, petId, orderId)

## 🧪 Negative Test Scenarios
- Create user with missing username → expect 4xx (currently returns 200 → defect).
- Add pet with invalid status → expect 4xx.
- Place order with negative quantity → expect 4xx.
- Get non-existing user → expect 404.
- Logout without login → expect 401 (but returns 200 → defect).

## 🧑‍💻 Author
*Neha Shende* | 💼 QA / Manual + API Tester
