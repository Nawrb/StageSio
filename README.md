#  Projet Docker – Environnement Conteneurisé

Ce projet permet de lancer rapidement un environnement conteneurisé à l’aide de **Docker Compose**.

---

## Installation

Assurez-vous d’être à la racine du projet (là où se trouve le fichier `docker-compose.yml`), puis lancez la commande suivante :

```bash
docker compose up -d

---

## Attention

Il est crucial que votre fichier de configuration s'appelle exactement Dockerfile et non Dockerfile.txt.

Si vous avez un problème d'extension sous Windows :

Ouvrez votre explorateur de fichiers.

Allez dans l'onglet Afficher.

Cochez la case Extensions de noms de fichiers.

Renommez le fichier pour supprimer le .txt s'il est présent.

---

## Résolution des problèmes

Erreur sur le Port **445**
Si vous rencontrez une erreur liée au port **445** lors du lancement, cela est généralement dû au service "Serveur" de Windows qui occupe ce port.

Procédure pour libérer le port :

Appuyez sur Windows + R.

Tapez services.msc et validez.

Cherchez le service nommé Serveur.

Faites un clic droit -> Propriétés.

Changez le type de démarrage sur Désactivé.

Cliquez sur le bouton Arrêter (en haut à gauche de la fenêtre des propriétés).

Relancez la commande docker compose up.
