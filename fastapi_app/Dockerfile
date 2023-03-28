FROM tiangolo/uvicorn-gunicorn-fastapi:python3.9-slim

COPY requirements.txt requirements.txt

RUN pip3 install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 80

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]
