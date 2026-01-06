#  Docker Samba

Ce projet permet de lancer rapidement un environnement conteneurisé à l’aide de **Docker Compose**.

---

## Installation

Assurez-vous d’être à la racine du projet (là où se trouve le fichier `docker-compose.yml`), puis lancez la commande suivante :

```bash
docker compose up -d
```
---

## Attention

Il est crucial que votre fichier de configuration s'appelle exactement Dockerfile et non Dockerfile.txt.

# Procédure Windows pour corriger l'extension :

1. Ouvrez l'explorateur de fichiers.

2. Accédez à l'onglet Affichage.

3. Cochez la case Extensions de noms de fichiers.

4. Renommez votre fichier pour supprimer le suffixe .txt s'il est présent.

---

## Résolution des problèmes

Erreur sur le Port **445**
Si vous rencontrez une erreur liée au port **445** lors du lancement, cela est généralement dû au service "Serveur" de Windows qui occupe ce port.

# Procédure pour libérer le port :

1. Appuyez sur Windows + R.

2. Tapez services.msc et validez.

3. Cherchez le service nommé Serveur.

4. Faites un clic droit -> Propriétés.

5. Changez le type de démarrage sur Désactivé.

6. Cliquez sur le bouton Arrêter (en haut à gauche de la fenêtre des propriétés).

Relancez la commande docker compose up.
