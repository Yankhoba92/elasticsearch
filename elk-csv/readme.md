# TP ELK-CSV

Ce TP permet d'ingérer des données CSV en utilisant la stack ELK (Elasticsearch, Logstash, Kibana) via Docker.

## Étapes à suivre

### 1. Installation d'un fichier `docker-compose.yml`

- **Mise en place des containers** : Lancez la commande suivante pour démarrer les services Elasticsearch, Logstash et Kibana avec Docker Compose :
    ```bash
    docker-compose up -d 
    ```

### 2. Vérification des services

Une fois les containers démarrés, tu peux vérifier leur état avec la commande suivante :
    ```bash
    docker-compose ps
    ```

### 3. Configuration du pipeline Logstash

Le pipeline Logstash est configuré pour ingérer deux types de données :

- **Fichier CSV** : Le fichier `data.csv` est ingéré, transformé en JSON, et indexé dans Elasticsearch sous l'index `orders-YYYY.MM.dd`.
  
- **Logs Apache** : Le fichier `apache_logs.txt` est traité pour extraire les informations avec un pattern `COMBINEDAPACHELOG` et indexé sous l'index `web_server_logs`.

Les fichiers de configuration nécessaires se trouvent dans les répertoires `logstash` et `elasticsearch` :
- `logstash.conf` : Définition du pipeline pour traiter les données.
- `elasticsearch.yml` : Configuration d'Elasticsearch.

### 4. Arrêter et nettoyer les containers

Si tu souhaites arrêter les containers, utilise la commande suivante :
    ```bash
    docker-compose down
    ```
Pour supprimer également les volumes et les données, exécute :
    ```bash
    docker-compose down -v
    ```

---

