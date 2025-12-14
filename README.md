Ce projet présente un prototype de Smart Farm basé sur l’Internet des Objets (IoT). Il combine une partie hardware (ESP32, capteurs, actionneurs, alimentation solaire) et une partie software (application mobile Flutter avec Supabase). L’objectif est de surveiller en temps réel les paramètres agricoles essentiels et d’automatiser certaines actions pour une gestion durable des ressources.

Fonctionnalités principales
Capteurs intégrés :
  DHT11 (température et humidité de l’air)
  DS18B20 (température sol/eau)
  MQ135 (qualité de l’air / gaz)
  BH1750 (luminosité)
  Capteur d’humidité du sol
  Capteur de niveau d’eau

Actionneurs :
  Relais moteur (pompe/ventilation)
  Buzzer (alerte sonore)
  LEDs indicatives (niveau d’eau, moteur ON)

Alimentation autonome :
  Panneau solaire
  Contrôleur de charge
  Batterie rechargeable

Application Flutter :
  Authentification sécurisée (login/signup via Supabase)
  Chatbot agricole interactif
  isualisation en temps réel des données via MQTT
  Notifications en cas de dépassement de seuils

Communication : 
  Transmission des données via WiFi et MQTT (broker HiveMQ).
  Format des données : JSON.
  Exemple :
  json
  {
    "lum": 300.5,
    "rhum": 60.0,
    "rtmp": 25.0,
    "dsTemp": 24.5,
    "water": 18,
    "soil": 45,
    "gas": 42
  }

Objectif
Mettre en place une solution IoT complète et durable pour l’agriculture intelligente, conciliant productivité, autonomie énergétique et interface utilisateur intuitive.
