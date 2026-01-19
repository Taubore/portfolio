+++
title = "LeRobot"
weight = 20
description = "Projet LeRobot (SO-101) de Hugging Face pour m'initier à la robotique de base et surtout au *Machine Learning*."
summary = "Exploration du bras robotique LeRobot (SO-101) pour comprendre le contrôle des servo-moteurs, la cinématique et le *Machine Learning*."
thumbnailImage = "lerobot_000.jpg"
date = 2026-01-14
tags = ["Robotique", "Intelligence artificielle", "Feetech STS3215", "Python"]
categories = ["Projets"]
status = "En cours"
+++

{{< figure
    src="lerobot_000.jpg"
    alt="Bras robotique LeRobot (SO-101)"
    width="50%"
>}}

## Informations clés
- **Type de projet** : Bras robotique avec IA
- **Objectif principal** : Aprentissage de la robotique et de l'intelligence artificielle
- **Principaux composants** : 12 servo-moteurs Feetech STS3215, 2 contrôleurs de servo-moteurs Waveshare
- **Système d'exploitation, langage et framework** : Linux, Python, LeRobot (PyTorch)
- **État** : en cours

## Description
Le projet LeRobot (SO-101) de Hugging Face vise à démocratiser la robotique en fournissant des modèles pré-entraînés, des jeux de données et des outils open source basés sur PyTorch. L’objectif est de réduire les barrières d’entrée et de permettre à chacun de contribuer et de bénéficier des avancées en apprentissage par imitation et en apprentissage par renforcement. 

*Source : https://huggingface.co/docs/lerobot/index*

Un peu d'investissment monétaire est toutefois requis pour ce projet, soit un total d'environ(~) 360 $ CAD :
- 12 servo-moteurs (~240 $ CAD) 
- 2 contrôleurs de servo-moteur (~30 $ CAD)
- 2 adaptateurs d'alimentation 5 V (~30 $ CAD)
- 2 câbles USB-C (~20 $ CAD)
- 1 kit de 4 supports (~20 $ CAD)
- Bobine de 1 Kg de PLA pour l'impression des pièces (~20 $ CAD)

## Détails composants
- Voir la [liste](https://github.com/TheRobotStudio/SO-ARM100?tab=readme-ov-file#sourcing-parts) des composantes sur le site officiel
    - [SeeedStudio](https://www.seeedstudio.com/) vend un kit disponible sur demande chez [Robotshop](https://ca.robotshop.com/fr/products/seeed-studio-so-arm101-kit-pro-moteur-servo-ai-pour-lerobot-sans-pieces-imprimees-en-3d?qd=86ec28df13519b4e2822530b72557d28) ou directement depuis le site de cette entreprise
- Imprimante 3D pour les [pièces](https://github.com/TheRobotStudio/SO-ARM100/tree/main/STL/SO101)
    - J'ai utilisé du simple [PLA Eryone](https://www.amazon.ca/-/fr/dp/B07ZPT32M8/?coliid=I66YM9SVIHF5W&colid=2W07VLY5OZPYW&ref_=list_c_wl_lv_ov_lig_dp_it&th=1)
    - Pas d'imprimante 3D ? [SeeedStudio](https://www.seeedstudio.com/) vend les pièces déjà imprimées pour les deux bras. Ce kit est disponible sur demande chez [Robotshop](https://ca.robotshop.com/fr/products/seeedstudio-so-arm101-ai-arm-pieces-imprimees-en-3d?qd=990071e8b3c694f2b8b0efde2e903a45) ou directement depuis le site de cette entreprise

## Chronologie

### 2025-12-23 - Bras *follower* presque terminé
{{< figure
    src="lerobot_001.jpg"
    alt="Lerobot *follower*"
>}}
La construction semble terminée, mais pas tout à fait. Il me reste encore quelques pièces à assembler.

### 2026-01-02 - Bras *follower* finalisé et testé
{{< figure
    src="lerobot_002.jpg"
    alt="Lerobot *follower* avec pièces pour le *leader*"
>}}
Le bras *follower* est maintenant terminé, branché, calibré et testé. Les 6 moteurs Feetech et les pièces pour le *leader* sont imprimés en plastique PLA.

### 2026-01-18 - Bras *leader* finalisé et testé
{{< figure
    src="lerobot_003.jpg"
    alt="Lerobot *leader* construit, branché, calibré et testé."
>}}
Le bras *leader* est maintenant terminé, branché, calibré et testé. Quelques soucis lors de la calibration. Je n'avais pas centré la position de mes moteurs avec [l'outil de test de Feetech](https://www.feetechrc.com/software.html) avant l'assemblage. Lors de la calibration, j'ai eu une erreur et j'ai donc dû démonter chaque articulations pour repositionner chaque moteur au centre et remettre la pièces au bon endroit.

### 2026-01-18 - Premier essais avec le bras *follower*
{{< youtube id="maZ5j3GNaw8" >}}
Premier essais de mouvements du bras *follower* à partir d'un enregistrement fait avec le bras *leader*. Un programme en Python enregistre un fichier CSV avec des mouvements que j'ai effectués manuellement pendant 10 secondes sur le bras *leader*. Un second programme Python lit le fichier CSV et reproduit ce mouvement sur le bras *follower*. C'est ce que représente cette vidéo. Encore aucune utilisation d'intelligence artificielle. Le programme Python est aussi très basique et ne fait aucune compensation de latence. Je vais publier ce code prochainement.



