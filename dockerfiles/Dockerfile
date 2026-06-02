from python:3.12-slim
workdir /app
copy requirements.txt .
run pip install --no-cache-dir -r requirements.txt
run useradd -m appuser 
USER appuser
copy app.py .
expose 5000
cmd ["python", "app.py"]
