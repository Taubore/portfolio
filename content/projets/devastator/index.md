+++
title = "Devastator"
weight = 20
description = "Mon robot expérimental qui m'aide à apprendre l'électronique et divers capteurs ainsi que le framework ROS 2."
summary = "Robot mobile expérimental pour l’apprentissage de l’électronique et de ROS 2."
thumbnailImage = "Devastator_001.jpg"
date = 2026-01-14
tags = ["Robotique", "Raspberry Pi 5", "ESP32", "DFRobot", "ROS 2", "Python"]
categories = ["Projets"]
status = "En cours"
+++

## Informations clés
- **Type de projet** : Robot mobile expérimental
- **Objectif principal** : Apprentissage de l’électronique et de ROS 2
- **Principaux composants** : Raspberry Pi 5, ESP32, utilisation d'une partie du kit Devastator de DFRobot
- **Système d'exploitation, langage et framework** : Linux, Python, ROS 2
- **État** : en cours

## Description
Robot expérimental qui m'aide à apprendre ROS 2 et la robotique en général. Initialement bâti à partir du kit [Devastator de DFRobot](https://www.dfrobot.com/product-1477.html). Aujourd'hui je n'utilise maintenant que les chenilles de cette plateforme.

## Détails composants
- Chenilles du kit [Devastator de DFRobot](https://www.dfrobot.com/product-1477.html)
- Raspeberry Pi 5
- ESP32 
- 2 Moteurs DC 6V [DFRobot avec encodeur en quadrature (FIT0521)](https://www.dfrobot.com/product-1617.html)

## Chronologie
{{< figure
    src="Devastator_001.jpg"
    alt="Robot Devastator modifié avant déconstruction partielle"
    caption="2025-12-12 : Ancienne configuration peu avant déconstruction partielle, car je prévois une réfonte au niveau de l'alimentation."
>}}

{{< figure
    src="Devastator_002.jpg"
    alt="Robot Devastator modifié vue de face"
    caption="2025-12-22 : Après déconstruction partielle. Devant il y a un capteur de distance à ultrason (Seeed Studio - Grove - Ultrasonic Ranger V2.0). Derrière le panneau avant (zone trouée), il y a un haut parleur (Visaton BF 37 8 Ohms)."
>}}

{{< figure
    src="Devastator_003.jpg"
    alt="Robot Devastator modifié vue du dessus"
    caption="Raspberry Pi5 en haut à gauche. À droite un ESP32. Mon intention est de faire du ESP32 mon contrôleur de moteur avec notamment la gestion de l'encodeur. Le Raspebrry Pi donnera les ordres au ESP32 pour tout ce qui se rapporte aux moteurs."
>}}

{{< figure
    src="Devastator_004.jpg"
    alt="Robot Devastator modifié capot ouvert, vue sur les moteurs"
    caption="Capot ouvert. Deux moteurs DFRobot 6 V avec encodeur en quadrature (FIT0521)"
>}}

## Vidéos
(à venir)
