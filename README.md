# QA-Cart — API Testing

![API Tests](https://github.com/Amira-Ouislati/QA-Cart/actions/workflows/main.yml/badge.svg)

Ce projet contient une collection de tests API développée sur l'application 
pédagogique [QA Cart](https://todo.qacart.com), une todo list conçue pour 
pratiquer les tests logiciels.

L'idée était de couvrir un parcours utilisateur complet, de l'inscription 
jusqu'à la suppression d'une tâche, en passant par l'authentification 
et les opérations CRUD.

## Scénario testé

| Méthode | Endpoint | Description |
|---------|----------|-------------|
| POST | /users/register | Inscription et récupération du token |
| POST | /tasks | Création d'un todo |
| PUT | /tasks/:id | Marquer la tâche comme complétée |
| DELETE | /tasks/:id | Suppression de la tâche |
| GET | /seed | Réinitialisation de la base de données |

## Stack

- Postman pour la conception et l'exécution des tests
- Postman CLI pour l'intégration en pipeline
- GitHub Actions pour déclencher les tests à chaque push
- Variables d'environnement pour gérer le token d'authentification

## Rapport d'exécution

[Voir le dernier run sur Postman Cloud](https://go.postman.co/workspace/e6f099ae-9b95-4f36-8732-299543c5592f/run/42769339-0b1e1704-f83f-405e-9e08-e05b4cf24ee5)


postman collection run "42769339-9ad6ee86-104c-4867-9330-e7e634a7903e" \
  -e "42769339-dcdc8ba3-3a29-4cb3-9041-b04dd69ee4b7"
```
