# docker-flask-gunicorn
Docker Image Template for flask + gunicorn

## Usage
1. `docker compose up --build`
2. Update requirements.txt as needed.
3. Run the container, mount the 'flask app' folder to the 'app' folder. For example: `docker run -itd --name my_flask_app -p 8000:8000 -v /path/to/my_flask_app:/app image_id`

- The 'flask app' folder should contain gunicorn_config.py (gunicorn settings file) and app.py (Flask app entry).
