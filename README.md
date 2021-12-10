# HerokuFlaskApp

Une fois le tout installer dans un dossier il suffit de build l'image et lancer le conteneur :

docker build -t flask-heroku:latest .

docker run -d -p 5000:5000 flask-heroku

puis une fois rendu à l'adresse : http://localhost:5000/, une page blanche avec "Flask Dockerized and deployed to Heroku" marqué devrait apparaitre.
