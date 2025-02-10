FROM python:3.11
WORKDIR /privilege
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt  
COPY . .  
EXPOSE 8050
CMD gunicorn --workers=4 --bind 0.0.0.0:8050 app:app