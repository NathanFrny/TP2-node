# TP2 Node.js

Nathan Fourny  

## Comment utiliser ?

### Lancer le projet

> Ouvrez vscode  
> Ouvrez un terminal dans la root du projet  
> Effectuez la commande suivante : "npm run start"

## PORT

> Le port par défaut du serveur express est 3000.  

## Test API

> Entrez l'url http://localhost:PORT/movie/:nomFilm  
> Vous serez redirigez vers une page affichant le résultat json de la requête API  

## Présentation Pug

> Entre l'url http://localhost:PORT/presentation  
> Vous pouvez testez les différents get disponible de l'API  

## Fonctions minimales

### Ajouter un Utilisateur

> Utilisez Postman
> Sélectionnez la requête http "POST"  
> Utilisez l'url http://localhost:PORT/user/add  
> Indiquez les éléments à créer dans la collection User (json = référe vous au schéma présent dans repositories/jsonSchema.js)  

### Afficher un Utilisateur

> Utilisez l'url http://localhost:PORT/user/get/:id  
> Utilisez l'url http://localhost:PORT/user/get (Permet de récupérer tous les utilisateurs)  

### Ajouter un Item

> Utilisez Postman
> Sélectionnez la requête http "POST"  
> Utilisez l'url http://localhost:PORT/item/add  
> Indiquez les éléments à créer dans la collection Item (json = référe vous au schéma présent dans repositories/jsonSchema.js)  

### Afficher un Item

> Utilisez l'url http://localhost:PORT/item/get/:id  

### Ajouter une watchlist

> Utilisez Postman
> Sélectionnez la requête http "POST"  
> Utilisez l'url http://localhost:PORT/watchlist/add  
> Indiquez les éléments à créer dans la collection Watchlist (json = référe vous au schéma présent dans repositories/jsonSchema.js)  

### Afficher une watchlist

> Utilisez l'url http://localhost:PORT/watchlist/get/:id (Permet de récupérer à partir de l'id d'une watchlist)  
> Utilisez l'url http://localhost:PORT/watchlist/get/user/:id (Permet de récupérer à partir de l'id d'un utilisateur)  


### Ajouter un Item dans une Watchlist

> Utilisez Postman  
> Sélectionnez la requête http "POST"  
> Utilisez l'url http://localhost:PORT/watchlist/addItem/:id (id de la watchlist)  
> Indiquez les éléments d'item à rajouter dans la watchlist (se référer à la section item dans le schéma de la watchlist -> Attention à bien créer l'item avant de l'ajouter dans la watchlist)  

### Modifiez le status d'un Item dans une Watchlist

> Utilisez Postman  
> Sélectionnez la requête http "POST"  
> Utilisez l'url http://localhost:PORT/watchlist/updateItemStatus/:watchlistId/:itemID   
> Indiquez le status de l'item (référez-vous aux status stocké dans le schéma de la watchlist)   


## Fonctions Supplémentaires

## Supprimer une Watchlist

> Utilisez Postman  
> Sélectionnez la requête http "DELETE"  
> Utilisez l'url http://localhost:PORT/watchlist/delete/:watchlistId  

## Modifier les informations personnelles d'un utilisateur

> Utilisez Postman  
> Sélectionnez la requête http "POST"  
> Utilisez l'url http://localhost:PORT/user/updatePersonalInfo/:userID  
> Entrez les informations personnelles dans un json (référez-vous au schéma dans jsonSchema.js)  

## Mettre une Watchlist en favori

> Utilisez Postman  
> Sélectionnez la requête http "POST"  
> Utilisez l'url http://localhost:PORT/watchlist/setFavorite/:watchlistId  
> Entre la valeur de "isFavorite" dans un json (true ou false)  
