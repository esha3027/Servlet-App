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
Servlet App/
├── src/
│   ├── main/
│       ├── java/
│           └── MainServlet.java
│       └── webapp/
│           ├── META-INF/
│               └── MANIFEST.MF
│           └── WEB-INF/
│               └── web.xml
```

2. **Add Servlet Mapping in `web.xml`:**
```xml
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         version="5.0">
    <servlet>
        <servlet-name>MainServlet</servlet-name>
        <servlet-class>MainServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>MainServlet</servlet-name>
        <url-pattern>/welcome</url-pattern>
    </servlet-mapping>
</web-app>
```

3. **Deploy on Tomcat:**
- Copy project to webapps folder.
- Start Tomcat.

---

## ✍️ Author Notes
This project is part of foundational training in Java Web Development using Jakarta Servlets. A great starting point for learners exploring server-side Java programming.

---
