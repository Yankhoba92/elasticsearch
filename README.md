Elasticsearch TP

Ce dépôt contient plusieurs travaux pratiques (TP) liés à l'utilisation et la configuration d'Elasticsearch.

Structure du projet

Le dossier Elasticsearch est organisé en plusieurs sous-dossiers, chacun correspondant à un TP spécifique :

Monitoring : Mise en place de la surveillance d'un cluster Elasticsearch.

elk-stack : Installation et configuration de la suite ELK (Elasticsearch, Logstash, Kibana).

elk-csv : Importation et manipulation de fichiers CSV dans Elasticsearch.

multiplePipeline : Gestion et utilisation de pipelines multiples dans Logstash.

search-elastic : Implémentation de recherches avancées avec Elasticsearch.

Prérequis

Avant de commencer, assurez-vous d'avoir installé les éléments suivants :

Docker et Docker Compose (recommandé pour la plupart des TP)

Java 8+ (si installation manuelle d'Elasticsearch)

Elasticsearch, Logstash et Kibana (versions compatibles avec les TP)

Installation et utilisation

Chaque TP contient ses propres fichiers de configuration et instructions d'utilisation.
Reportez-vous aux README respectifs dans chaque sous-dossier pour plus de détails.

Exécution avec Docker

Si un TP dispose d'un fichier docker-compose.yml, vous pouvez démarrer l'environnement avec :

cd <nom_du_tp>
docker-compose up -d

Arrêt de l'environnement

docker-compose down



Auteur

Yankhoba Bagayoko

N'hésitez pas à proposer des améliorations ou à signaler des problèmes via des issues !

