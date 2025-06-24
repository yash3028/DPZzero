FROM python:latest

WORKDIR /app

COPY . .

RUN pip install uv

RUN  pip install flask

EXPOSE 8002

CMD ["uv", "run", "app.py"]
