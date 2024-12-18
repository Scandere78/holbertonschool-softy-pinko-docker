FROM ubuntu:latest

# Installer Python et Flask
RUN apt-get update && apt-get install -y python3 python3-pip
RUN pip3 install flask flask-cors

# Définir le répertoire de travail
WORKDIR /app

# Copier le code source
COPY ./back-end /app

# Exposer le port
EXPOSE 5252

# Commande pour exécuter l'application
CMD ["python3", "api.py"]
