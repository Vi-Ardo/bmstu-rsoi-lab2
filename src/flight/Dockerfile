FROM python:3.11
WORKDIR /flight
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt  
COPY . .  
EXPOSE 8060
CMD gunicorn --workers=4 --bind 0.0.0.0:8060 app:app