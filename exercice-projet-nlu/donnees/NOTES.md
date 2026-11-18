# Notes sur les données

## Sujet et périmètre

Ces données servent à reconnaître six types de demandes courtes d'un voyageur
au Japon : itinéraires, hébergements, restaurants, visites, coutumes et services
pratiques. Le modèle produit une intention et, quand le message en contient, des
slots copiés du message. Il ne génère pas de conseils touristiques libres.

## Source et licence

Les phrases ont été rédigées synthétiquement pour cet exercice. Aucun jeu de
données externe ni donnée personnelle n'a été utilisé. Il n'y a donc pas de
licence tierce à attribuer.

## Choix d'annotation

- Les valeurs de slots sont en minuscules et reprises du message.
- `lieu_depart` et `lieu_arrivee` ne sont utilisés que pour les demandes
  d'itinéraire.
- `ville` identifie le lieu de la demande, `date` sa période et `critere` le
  sujet ou la préférence précisés (par exemple « végétarien », « onsen » ou
  « consigne »).
- Les demandes de coutumes sont distinguées des visites : une question sur les
  usages reçoit `coutumes`, une recherche de lieu ou d'activité reçoit `visite`.

## Limites

Les exemples couvrent surtout des lieux et formulations liés au Japon. Le jeu
est petit et synthétique : il ne garantit pas la généralisation aux variantes
régionales, aux fautes nombreuses, aux messages ambigus ou aux conversations
longues. Les réponses structurées ne doivent pas être présentées comme des
informations de voyage vérifiées ou actualisées.

## Évaluation

Le test local est un jeu tenu à part pour l'évaluation finale. Nombre de lectures
du test à la rédaction de ces notes : 0. Remplacer cette valeur après tout
lancement de `make juger`. Le test croisé pour un autre groupe reste à rédiger
séparément à partir de l'ontologie qui lui sera confiée.
