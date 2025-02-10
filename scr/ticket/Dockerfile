FROM python:3.11
WORKDIR /ticket
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt  
COPY . .  
EXPOSE 8070
CMD gunicorn --workers=4 --bind 0.0.0.0:8070 app:app