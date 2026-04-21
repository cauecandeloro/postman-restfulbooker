# API Testing - Restful Booker

API test collection for the [Restful Booker](https://restful-booker.herokuapp.com) booking system using Postman.

---

## About the Project

Restful Booker is a public REST API built for testing purposes. This project covers the main CRUD operations with automated API tests, including authentication, validation of response bodies, status codes, and dynamic variable management between requests.

## Tech Stack

- [Postman](https://www.postman.com/) — API testing tool
- JavaScript — test scripts
- Collection Runner — automated test execution

## Test Coverage

| Module | Scenarios |
|---|---|
| Auth | Generate authentication token |
| Bookings | Get all bookings, get booking by ID |
| Create Booking | Create booking with valid data, validate response body |
| Update Booking | Update existing booking, validate updated fields |
| Delete Booking | Delete existing booking, validate response status |

## Project Structure

postman-restfulbooker/
├── restfulbooker-collection.json
├── restfulbooker-environment.json
└── README.md

## How to Run

**Prerequisites:** Postman installed

1. Clone this repository
2. Open Postman
3. Import `restfulbooker-collection.json` via **File → Import**
4. Import `restfulbooker-environment.json` via **File → Import**
5. Select `Restful Booker - Environment` in the environment dropdown
6. Open the collection and click **Run collection**

## Key Concepts Demonstrated

- Authentication via token stored as collection variable
- Dynamic variables passing data between requests (`booking_id`, `new_booking_id`, `token`)
- Response body validation with JavaScript test scripts
- Full CRUD cycle — Create, Read, Update, Delete
