# 🚀 Nginx + PHP-FPM + PHP CLI + MySQL + Vue.js (Dockerized)

This project sets up a **PHP API with Nginx, PHP-FPM, PHP CLI, and MySQL**, alongside a **Vue.js frontend**, using **Docker Compose**.  


### **📌 Project Description**  

This project is a **Dockerized full-stack web application** integrating **Nginx, PHP-FPM, PHP CLI, MySQL, and Vue.js**. It provides a seamless development and deployment environment for building modern web applications with a **PHP backend** and a **Vue.js frontend**.  

With **Docker Compose**, the entire setup is automated, making it easy to start development without worrying about server configurations.  

---

### **🌟 Features**  
- **Nginx** – Serves Vue.js frontend & routes API requests  
- **PHP-FPM** – Processes backend PHP requests efficiently  
- **PHP CLI** – Dedicated for running PHP commands & scripts  
- **MySQL** – Stores application data with persistent storage  
- **Vue.js** – Dynamic and responsive frontend  
- **Docker Compose** – Simplifies multi-container management  

---

### **🎯 Use Cases**  
- Developing RESTful APIs with PHP  
- Single Page Applications (SPA) with Vue.js  
- Scalable and containerized web applications  
- Quick setup for PHP & JavaScript projects  

---

### **🚀 Quick Setup**  
1️⃣ Clone the repository  
```sh
git clone <repository-url>
cd <project-folder>
```  
2️⃣ Configure environment variables  
```sh
cp .env.example .env
```  
3️⃣ Start the application  
```sh
docker-compose up -d --build
```  

Visit **http://localhost/** for the frontend  
API available at **http://localhost/api/**  

---

### **📌 Why Use This Project?**  
✅ Fully **containerized** environment  
✅ **Easy to deploy** anywhere  
✅ Modern **tech stack**  
✅ Scalable & **production-ready**  

🚀 **Start building today!** 🚀  


---

## 📂 Project Structure
```
📂 project-root/ 
├── 📂 app/ # PHP API (Backend) │ 
    ├── index.php # Main API entry point │ 
    ├── config.php # Database connection │ 
    └── ... 
├── 📂 frontend/ # Vue.js Frontend │ 
    ├── 📂 src/ # Vue components & assets │ 
    ├── 📂 dist/ # Production build output │ 
    └── ... 
├── 📂 nginx/ # Nginx Configurations │ 
    ├── default.conf # Nginx server config 
├── 📄 docker-compose.yml # Docker Compose file 
├── 📄 .env # Environment variables 
├── 📄 README.md # Project documentation
```



---

## 🚀 Getting Started

### 1️⃣ **Clone the Repository**
```sh
git clone <repository-url>
cd <project-folder>
```

### 2️⃣ **Set Up Environment Variables**  
Create a `.env` file:
```sh
cp .env.example .env
```
Edit `.env` and configure MySQL, Nginx port, and PHP version.

### 3️⃣ **Start Docker Containers**
```sh
docker-compose up -d --build
```

---

## 🛠️ Services & Configuration

### 📌 **Docker Services**
| Service    | Description |
|------------|------------|
| `nginx`    | Serves Vue.js frontend & routes PHP API requests |
| `php`      | PHP-FPM for processing API requests |
| `php-cli`  | CLI container for executing PHP commands |
| `mysql`    | MySQL database for backend |

### 📌 **Nginx Configuration (`nginx/default.conf`)**
- `/` → Vue.js frontend (`dist/`)
- `/api/` → PHP backend (`index.php`)
- PHP requests handled via PHP-FPM

---

## 🖥️ Useful Commands

📦 **Start Containers**  
```sh
docker-compose up -d
```

🛑 **Stop Containers**  
```sh
docker-compose down
```

🔄 **Restart Containers**  
```sh
docker-compose restart
```

🐛 **View Logs**  
```sh
docker-compose logs -f nginx
```

---

## 🎯 API Endpoints (`/api/`)
| Method | Endpoint    | Description         |
|--------|------------|---------------------|
| `GET`  | `/api/`    | API test route      |
| `GET`  | `/api/users` | Fetch users        |

---

## 🎨 Frontend (Vue.js)

1️⃣ **Go to frontend directory**  
```sh
cd frontend
```

2️⃣ **Install dependencies**  
```sh
npm install
```

3️⃣ **Run Vue.js Development Server**
```sh
npm run dev
```

---

## 📌 License
This project is licensed under the MIT License.

---

## ✨ Author
Developed by **Mohammad Emran**  
🚀 Happy Coding!  
