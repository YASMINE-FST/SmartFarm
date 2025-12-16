🌱 Smart Farm IoT – AgriNova
📌 Description du projet

AgriNova est un projet de Smart Farm basé sur l’Internet des Objets (IoT), conçu pour améliorer la gestion des exploitations agricoles grâce à une surveillance en temps réel et une automatisation intelligente des paramètres environnementaux.
Le système combine une architecture matérielle basée sur ESP32 et une application mobile développée avec Flutter, permettant une gestion efficace, durable et connectée de l’agriculture moderne.

🎯 Objectifs

Surveiller en temps réel les paramètres environnementaux essentiels :

Température et humidité de l’air

Température du sol ou de l’eau

Humidité du sol

Luminosité

Qualité de l’air (gaz)

Niveau d’eau

Automatiser l’irrigation, les alertes et la ventilation selon des seuils prédéfinis

Réduire le gaspillage des ressources (eau et énergie)

Offrir une solution autonome énergétiquement grâce à l’énergie solaire

Proposer une interface mobile intuitive et sécurisée

🧠 Architecture du système
🔧 Partie matérielle (Hardware)

Microcontrôleur : ESP32 (Wi-Fi + MQTT)

Capteurs :

DHT11 (température et humidité)

DS18B20 (température sol/eau)

Capteur d’humidité du sol

Capteur de niveau d’eau

MQ135 (qualité de l’air)

BH1750 (luminosité)

Actionneurs :

Relais moteur (irrigation / ventilation)

Buzzer (alertes)

LEDs d’état (moteur actif, niveau d’eau bas)

Alimentation :

Panneau solaire

Contrôleur de charge

Batterie rechargeable

💻 Partie logicielle

Communication :

Wi-Fi

Protocole MQTT (Broker HiveMQ)

Application mobile (Flutter) :

Authentification sécurisée (Login / Signup)

Visualisation des données en temps réel

Historique des mesures

Chatbot agricole interactif

Backend & Base de données :

Supabase (authentification et stockage des données)

🔄 Fonctionnement

Les capteurs collectent les données environnementales en continu.
L’ESP32 traite ces données et :

Active automatiquement les actionneurs si les seuils sont dépassés (ex. gaz > 40 %, niveau d’eau < 20 %)

Publie les données au format JSON via MQTT
L’application Flutter affiche les données en temps réel et les stocke de manière sécurisée dans Supabase.

✅ Résultats

Transmission des données stable et en temps réel

Automatisation fiable de l’irrigation et des alertes

Interface mobile intuitive et sécurisée

Fonctionnement autonome grâce à l’énergie solaire
