FROM python:3.11
WORKDIR /gateway
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt  
COPY . .  
EXPOSE 8080
CMD gunicorn --workers=4 --bind 0.0.0.0:8080 app:app