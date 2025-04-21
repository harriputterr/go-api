# 🪙 Go API – Mock Coin Balance Service

This is a simple backend API built with **Go**, simulating a coin balance system using a mock database. It’s designed to showcase Go fundamentals such as routing, query decoding, modular structure, and structured logging — perfect for learning or portfolio projects.

---

## 🔧 Features

- ✅ RESTful API using `chi` router
- 🧪 Mock database to simulate user data
- 🧹 Clean modular file structure
- 📄 Query param decoding with `gorilla/schema`
- 🪵 Logging with `logrus`

---

## 📁 Folder Structure

`go-api/` contains the complete structure for the Go API project including handlers, mock database logic, middleware, and entry point. Here's a breakdown of what's inside:

```
go-api/
├── api/                  # Request/response types
├── internal/
│   ├── tools/            # Mock DB and setup logic
│   └── middleware/       # (Optional) Authorization middleware
├── handlers/             # Business logic for routes
├── cmd/
│   └── api/              # Entry point (main.go)
├── go.mod
├── go.sum
```

---

## 🚀 How to Run

```bash
git clone https://github.com/harriputterr/go-api.git
cd go-api
go run ./cmd/api
```

Then hit:

```
http://localhost:8000/balance?username=harsingh
```

---

## 📨 Example Response

```json
{
  "code": 200,
  "balance": 1000
}
```

Error case:

```json
{
  "code": 400,
  "message": "User not found"
}
```

---

## 🛠 Tech Stack

- [Go](https://golang.org/)
- [Chi Router](https://github.com/go-chi/chi)
- [Gorilla Schema](https://github.com/gorilla/schema)
- [Logrus](https://github.com/sirupsen/logrus)

---

## 🙌 Acknowledgement

Built as part of backend skill development and mock API simulation — helpful for learning Go and demonstrating backend structure in interviews or personal projects.

