# Case 1 : My answer
# FROM python:3.9

# WORKDIR /app

# RUN ["pip", "install", "flask"]

# COPY . .

# CMD ["python", "main.py"]

# docker run -p 5000:8000 httpd

# --------------------------------

# Case 2 : In "main.py", change port

# FROM python:3.9

# WORKDIR /app

# RUN pip install flask

# COPY . .

# EXPOSE 8000

# CMD ["python", "main.py"]

# --------------------------------

# Case 3 : docker run
FROM python:3.9

WORKDIR /app

RUN pip install flask

COPY . .

EXPOSE 5000

CMD ["python", "main.py"]

# docker run -p 8000:5000 flask-app 