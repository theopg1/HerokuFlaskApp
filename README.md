# HerokuFlaskApp

Une fois le tout installé dans un dossier il suffit de build l'image et lancer le conteneur :

`docker build -t flask-heroku:latest .`

`docker run -d -p 5000:5000 flask-heroku`

puis une fois rendu à l'adresse : http://localhost:5000/, une page blanche avec "Flask Dockerized and deployed to Heroku" marqué devrait apparaitre.

Ensuite pour déployer Heroku il faut dans un premier temps ce connecter avec la commande `heroku container:login`

Ainsi on peut créer son app avec `heroku create`

Et la vérifié avec `heroku apps`

Ensuite il faut créer le container avec `heroku container:push web --app [appname]`

Enfin il faut release le container avec `heroku container:release web --app [appname]`

On pourra donc enfin accéder à notre application Heroku via le lien https://[appname].herokuapp.com/ .
