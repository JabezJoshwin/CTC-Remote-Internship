# Apple-Inspired Landing Page 🚀

A clean, Apple-style responsive landing page for showcasing products (e.g., iPhone 16). Built using HTML and CSS.

---

## 📦 Run with Docker

This project uses **Nginx** in a Docker container to serve the static website.

---

## 🛠️ Prerequisites

- [Docker](https://www.docker.com/) installed on your system

---

## 📁 Project Structure

```
project-root/
│
├── index.html
├── styles.css
├── images/
│   └── iphone16.png
├── Dockerfile
└── README.md
```
---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/apple-landing-page.git
cd apple-landing-page
```
### 2.Build the Docker image
```bash
docker build -t apple-landing-page .
```

### 3. Run the Docker container
```bash
docker run -d -p 8080:80 apple-landing-page
```

### 4. Now open your browser and go to: http://localhost:8080 or [click here](http://localhost:8080)
