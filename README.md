# 🌐 Servlet Application

This is a minimal Java Servlet application developed with the **Jakarta Servlet API**. The application illustrates the minimal servlet lifecycle (`init()`, `doGet()`, and `destroy()`) and returns a welcome HTML page in response to GET requests.

---

## 📄 File Overview

- `MainServlet.java`: A minimal servlet that:
- Initializes upon server loading of the servlet.
- Processes HTTP GET requests by returning a simple HTML response.
- Cleans up resources upon servlet destruction.

---

## 🚀 How It Works

### Servlet Lifecycle Methods:
| Method | Purpose |
|--------------|----------------------------------------------|
| `init()` | Invoked once when initializing the servlet. |
| `doGet()` | Invoked for each HTTP GET request. |
| `destroy()` | Invoked once when shutting down the servlet. |

---

## 🧱 Requirements

- JDK 11+
- Apache Tomcat or any Servlet container (e.g., Jetty)
- Jakarta Servlet API (Jakarta EE 9+)

## ⚙️ How to Deploy

1. **Project Structure (within a Dynamic Web Project or WAR format):**
```pgsql
YourProject/
├── WEB-INF/
│   ├── web.xml
│   └── classes/
│       └── MainServlet.class
```
