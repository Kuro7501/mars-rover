FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir --upgrade pip setuptools \
 && pip install --no-cache-dir -r requirements.txt

COPY serveur.py .

EXPOSE 80
CMD ["python", "serveur.py"]
