### **AI-Based Resume Scanner**  
An AI-powered resume scanner that extracts and analyzes information from resumes using **Natural Language Processing (NLP)** and **Django**. The project is containerized using **Docker** for easy deployment.  


## **🚀 Features**  
✅ Extracts text from resumes  
✅ Analyzes and categorizes resume content  
✅ Web interface using **Django**  
✅ Dockerized deployment for easy setup  
✅ REST API for parsing resumes  


## **📁 Project Structure**  

```
AI-Based_Resume-Scanner/
│── nginx/                # Nginx configuration for reverse proxy
│   ├── Dockerfile        # Dockerfile for Nginx setup
│   ├── nginx.conf        # Nginx configuration file
│
│── results/              # Stores parsed resume results
│   ├── resume_parser_result.png  # Example output
│
│── resume_parser/        # Core resume parsing logic
│   ├── cli.py            # Command-line interface for parsing resumes
│   ├── Dockerfile        # Dockerfile for resume parser service
│   ├── pre_requisites.py # Pre-requisite setup
│   ├── requirements.txt  # Python dependencies
│
│── parser_app/           # Django application for web interface
│   ├── migrations/       # Database migrations
│   ├── static/           # Static files (CSS, JS)
│   ├── templates/        # HTML templates for UI
│   ├── templatetags/     # Django custom template tags
│   ├── __init__.py       # Marks this as a Python package
│   ├── admin.py          # Django admin panel configuration
│   ├── apps.py           # Django app configuration
│   ├── models.py         # Database models
│   ├── tests.py          # Unit tests
│   ├── urls.py           # URL routing
│   ├── views.py          # Business logic and API endpoints
│
│── .gitignore            # Files to ignore in version control
│── django.conf           # Django settings
│── docker-compose.yml    # Docker Compose for multi-container setup
│── manage.py             # Django management script
```


## **🔧 Installation & Setup**  

### **1️⃣ Clone the repository**  
```sh
git clone https://github.com/your-username/AI-Based_Resume-Scanner.git
cd AI-Based_Resume-Scanner
```

### **2️⃣ Install dependencies**  
```sh
pip install -r resume_parser/requirements.txt
```

### **3️⃣ Run Django migrations**  
```sh
python manage.py migrate
```

### **4️⃣ Start the Django server**  
```sh
python manage.py runserver
```

Now, open **http://127.0.0.1:8000/** in your browser to access the app.

---

## **🐳 Docker Setup**  
### **1️⃣ Build and start containers**  
```sh
docker-compose up --build
```
### **2️⃣ Access the app**  
Once running, access the app at **http://localhost/**.


## **📌 API Endpoints**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/parse-resume/` | Upload and parse a resume |
| `GET`  | `/results/` | View parsed resume results |


## **🛠 Technologies Used**  
- **Python, Django** – Web framework  
- **NLP, Spacy** – Resume parsing  
- **Docker, Docker Compose** – Containerized deployment  
- **Nginx** – Reverse proxy  


## **🤝 Contributing**  
Feel free to fork this repo, submit issues, or create pull requests!  


### **📜 License**  
This project is licensed under the **MIT License**.
