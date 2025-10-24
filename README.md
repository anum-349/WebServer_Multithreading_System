# 🌐 Multithreaded Web Server – C++

A **simple multithreaded HTTP web server** built in C++ for serving static files using Winsock on Windows. Supports multiple simultaneous clients with **GET request handling**.

---

## 🛠️ Features

* **Multithreading**: Each client connection is handled in a separate thread using `std::thread`.
* **HTTP GET Support**: Serves only `GET` requests for static files.
* **File Serving**: Serves files from a `www` directory. Automatically serves `index.html` for directory requests.
* **404 Handling**: Returns `404 Not Found` for missing files.
* **Cross-file Directory Support**: Can serve HTML, CSS, JS, images, or other static files placed in the base directory.

---

## 🛠️ Technologies Used

* **C++17** – Programming language
* **Winsock2** – Windows networking API
* **Multithreading (`std::thread`)** – Handle multiple clients concurrently
* **Filesystem (`<filesystem>`)** – Manage server directories and file paths
* **Standard File I/O** – Serve content from static files

---

## 📂 Project Structure

```
WebServer_Multithreading_System/
│
├── Web server.cpp            # Main C++ server code
├── Web server.sln            # Visual Studio solution
├── Web server.vcxproj        # Visual Studio project file
├── Web server.vcxproj.filters
├── Web server.vcxproj.user
├── www/                      # Base directory for serving files
│   └── index.html            # Example homepage
```

---

## 🚀 How to Run

1. **Clone the repository**:

```bash
git clone https://github.com/anum-349/WebServer_Multithreading_System.git
```

2. **Open the project in Visual Studio** and build it.

3. **Ensure a `www` folder exists** in the project directory containing `index.html` or other static files.

4. **Run the server**:

   * The server listens on **port 8080**.
   * Open a browser and navigate to:

     ```
     http://localhost:8080/
     ```

5. **Access other files** by placing them in the `www` folder and navigating to:

```
http://localhost:8080/filename
```

---

## 🎯 Outcome

* The server can **handle multiple clients simultaneously** using multithreading.
* Demonstrates **network programming** with Winsock and **C++ file I/O**.
* Serves static files efficiently and handles basic HTTP requests.

---

## 📌 Skills Highlighted

**C++ · Winsock Networking · Multithreading · HTTP Protocol · File Management · Console Application Development**
