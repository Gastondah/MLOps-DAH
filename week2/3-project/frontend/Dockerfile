FROM python:3.10-slim

LABEL maintainer="Gaston Horace <gaston.horace@example.com>"

WORKDIR /app
COPY requirements.txt .
RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt
COPY . .

EXPOSE 8501
CMD ["streamlit", "run", "frontend.py", "--server.port", "8501", "--server.address", "0.0.0.0"]