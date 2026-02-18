# My Django Project

A simple Django practice project containerized using Docker.

This project is designed for learning and experimentation with Django while keeping the setup extremely simple. 
Everything runs inside Docker containers, so no local Python or dependency installation is required.

---

## 🚀 Quick Start (One Command)

Make sure Docker is running, then:

```bash
docker compose up
```

That’s it 🎉

Open your browser and enter the below address :

http://127.0.0.1:8000

---

## 🐳 Requirements

Install:

- Docker
- Docker Compose (usually bundled with Docker Desktop)

Verify:

```bash
docker --version
docker compose version
```

---

## 📦 What This Project Includes

- Django web application
- Dockerized environment
- Automatic dependency setup
- Development server inside a container
- SQLite database (default)

---

## 📁 Project Structure

```
my_django_project/
│
├── docker-compose.yml   # Multi-container configuration
├── Dockerfile          # App container definition
├── manage.py
├── requirements.txt
├── app/ or project/    # Django source code
└── README.md
```

---

## 🛠 Useful Commands

### Start the app

```bash
docker compose up
```

### Run in background

```bash
docker compose up -d
```

### Stop containers

```bash
docker compose down
```

### Run Django commands inside the container

```bash
docker compose exec web python manage.py migrate
docker compose exec web python manage.py createsuperuser
```

---

## 🔧 Development Notes

- Code changes auto-reload the server (if volumes are mounted)
- No need to install Python/Django locally
- Everything runs inside Docker for consistency

---

## 📚 Learning Goals

This project helps practice:

- Django apps, models, views, templates
- Routing (URLs)
- Admin panel usage
- Dockerizing a web application
- Running Django in containers

---

## 🤝 Contributing

Feel free to:

- Add new features
- Improve Docker setup
- Add tests
- Improve documentation

---

## 📄 License

For learning and personal use.
