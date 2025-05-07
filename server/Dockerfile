FROM python:3.10-slim
WORKDIR /app
RUN apt update && apt install -y curl && apt clean
RUN curl -sSL http://install.python-poetry.org | python3 - && \
echo "export PATH="/root/.local/bin:$PATH"' >> ~/.bash
COPY . .
CMD ["python","manage.py","runserver","0.0.0.0:8080"]
EXPOSE 8000
ENV PATH="/root/.local/bin:$PATH"
