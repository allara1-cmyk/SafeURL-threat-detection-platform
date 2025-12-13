## Backend Setup

### 1. Create virtual environment
python -m venv venv
venv\Scripts\activate

### 2. Install dependencies
pip install -r requirements.txt

### 3. Run PostgreSQL with Docker
cd docker
docker compose up -d

### 4. Apply migrations
python manage.py makemigrations
python manage.py migrate

### 5. Run server
python manage.py runserver
