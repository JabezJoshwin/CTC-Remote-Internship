FROM python:3.9-slim

WORKDIR /app

COPY ../templates/ /app/
COPY ../styles.css /app/
COPY ../images/ /app/images/
COPY ../script.js /app/

EXPOSE 3000

CMD ["python3", "-m", "http.server", "3000"]
