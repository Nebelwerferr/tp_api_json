  # Ping API

## Description
Cette API retourne les headers de la requête HTTP GET sur `/ping` au format JSON. Toute autre requête renvoie une réponse vide avec un code 404.

## Configuration du port
Le serveur écoute sur un port défini par la variable d'environnement `PING_LISTEN_PORT`. Par défaut, il écoute sur le port **3000**.

---> Pour modifier le port remplacer la valeur par celle souhaité 

```powershell
$env:PING_LISTEN_PORT = 3000   
```

## Démarrer le serveur

```powershell
npm start
```
Le serveur sera accessible sur `http://localhost:<port>`.

## Tester l'API
Avec `curl` :
```powershell
curl http://localhost:3000/ping
```
---> Retourne un fichier JSON avec le header de la requête.
