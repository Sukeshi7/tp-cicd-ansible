# Image de base officielle Python
FROM python:3.11

# Définir le dossier de travail
WORKDIR /app

# Copier les dépendances et les installer
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copier le reste des fichiers de l'app
COPY . .

# Exposer le port Flask
EXPOSE 5000

# Lancer l'app
CMD ["python", "app.py"]
