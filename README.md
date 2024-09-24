# STM32F407_CAN_Intercom


** Introduction : 

Ce projet démontre une communication simple mais efficace entre deux microcontrôleurs STM32F407 via le protocole CAN, en utilisant le transceiver MCP2551 pour assurer une isolation galvanique et une adaptation de niveau. Lorsqu'un événement se produit sur l'un des microcontrôleurs (par exemple, un bouton pressé), un message CAN est envoyé et déclenche une action sur l'autre microcontrôleur (par exemple, l'allumage de LED).

** Matériel nécessaire : 

2 cartes STM32F407 (ou équivalent)

2 transceivers MCP2551

2 résistances de pull-up (120 ohms typiquement)

Fils de connexion

** Logiciel nécessaire : 

Environnement de développement pour STM32 (e.g., STM32CubeIDE)



** Fonctionnement : 

Initialisation:
Configuration des périphériques CAN sur les STM32F407 (vitesse de bit, mode de fonctionnement, filtres).

Transmission:
Lorsqu'un événement se produit, un message CAN est préparé et envoyé via le MCP2551.

Réception:
Les interruptions sont utilisées pour détecter l'arrivée de nouveaux messages CAN.
Le message reçu est analysé et les actions correspondantes sont exécutées.

****** Editor : BenazizaAya ******
