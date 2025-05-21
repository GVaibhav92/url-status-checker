# 🌐 URL Status Checker (Go)

A simple and concurrent CLI tool written in Go that checks the HTTP status of a list of websites in real-time and re-checks them periodically. Useful for monitoring website uptime and latency.

---

##  Features

-  Checks the availability (HTTP status) of URLs
- ⏱️ Measures response time (latency)
- 🔄 Automatically rechecks links every few seconds
-  Uses Go's goroutines and channels for concurrency
-  Lightweight and fast

The program will:

-> Ping a set of hardcoded URLs
-> Print their status and response time
-> Re-check each URL every 3 seconds indefinitely

🔍 How It Works

* Each URL is checked in a separate goroutine
* A channel is used to queue the next check after 3 seconds
* HTTP GET requests measure status and latency














