# Introduction

La réunion a été ouverte avec un rappel des objectifs des sessions précédentes du CNIG, visant à faire le point sur les avancées réalisées depuis la création du RNB en avril 2022. L’objectif principal est de fédérer une communauté autour d’un standard de données bâties en France, impliquant des acteurs du secteur public, privé et associatif. Environ 25 entités ont participé aux groupes de travail, comprenant des représentants de communes, d'agences publiques et d'organisations privées.

# Avancées du RNB depuis la dernière session en Novembre 2023

- **Usages de la définition du bâtiment**
    - L'élaboration d'une définition partagée du bâtiment a depuis été adoptée par de nombreux acteurs et différents services au sein des métropoles. Cette définition permet déjà dans un premier temps d'harmoniser les différentes pratiques et d'assurer une cohérence dans la gestion des données relatives aux bâtiments.
- **Initialisation et mise en œuvre du référentiel** :
    - Le référentiel a été initialisé et nécessite maintenant d'être alimenté et mis à jour régulièrement via des contributions et des flux de données.
    - Un service de diffusion a été mis en place pour que le RNB soit utilisé par différentes bases de données (comme la BDNB du CSTB, la BD Topo de l'IGN, etc.).
- **Intégration dans différentes bases de données** :
    - Les identifiants du RNB sont déjà présents dans diverses bases, y compris celles des équipements sportifs du ministère de l'Enseignement supérieur et des sports, et dans des projets comme les DPE (Diagnostics de Performance Energétique) très prochainement.
    - Des efforts sont en cours pour diffuser ces identifiants dans d'autres bases de données, y compris OpenStreetMap (OSM).
- **Outils et API** :
    - Des API ont été mises en place pour faciliter l'intégration des informations du RNB dans les bases de données des différents acteurs.
    - Des expérimentations sont menées auprès de certains éditeurs de logiciels pour voir si ces outils permettent de sélectionner ou de pointer des bâtiments futurs, dès le début d'un projet.
- **Signalements et corrections** :
    - Un outil de signalement a été déployé, permettant aux utilisateurs de signaler des erreurs (comme des adresses incorrectes ou des informations manquantes sur les bâtiments).
    - Ce système est encore en phase de test, et des améliorations sont prévues pour faciliter la gestion des contributions et des signalements.
- **Officialisation**
    - **Le RNB est également une "Donnée de forte valeur" selon la Commission européenne.** Dans la lignée de la «**Directive Open Data**» (Directive 2019/1024), la Commission européenne a adopté un règlement d’exécution (2023/138) qui établit **la liste des ensembles de données de forte valeur, dont le Référentiel National de Bâtiments fait partie.**

# Echanges du jour

## Les contributions au RNB

Un des sujets centraux de la réunion a été les processus de contribution au référentiel. Les participants ont souligné l'importance de créer un système qui permet de recueillir les contributions de divers acteurs tout en garantissant la qualité et la fiabilité des données.

L’équipe du RNB a présenté [les premiers résultats du "jeu de l'été"](https://rnb.beta.gouv.fr/blog/jeu-concours-de-lete-quels-apprentissages-pour-le-rnb), qui visait à **contribuer à la qualité du RNB** à travers un module de signalement des erreurs dans la base de données du référentiel. Voici un résumé des principaux résultats :

- **Participation massive** : Plus de 120 participants ont contribué, bien plus que prévu intialement, avec **8 300 contributions** concernant des erreurs ou des suggestions de modification dans la base.
- **Erreurs identifiées** : Les erreurs les plus fréquentes concernaient la fusion ou la division des bâtiments (par exemple, deux bâtiments distincts ou un bâtiment divisé à tort), des bâtiments légers incorrectement enregistrés, et des adresses mal associées aux bâtiments. Un biais a néanmoins été introduit par le fait que le jeu poussait d’avantage au volume de contributions, qui temps à mettre en avant d’avantages les problèmes liés aux fusions et divisions.
- **Conséquences** : Cela a permis de corriger massivement la base de données et de mieux représenter le parc bâti, facilitant le croisement d'informations avec d'autres bases de données.

Il a été proposé de développer un processus clair pour la mise à jour régulière des données. Cela englobe la correction d'adresses erronées, la géolocalisation précise des bâtiments et la mise à jour de leur statut, comme les constructions ou les démolitions. Le groupe a convenu que ces mises à jour devaient être effectuées de manière fiable et régulière pour que le RNB reste pertinent et utile.

- Quelques questions ont été posées au participants sous forme de sondage
    - Est ce que ca bloquerai mon usage si le RNB était ouvert largement aux contributions ?
        - Pas du tout, c'est une force: 7 ||||||| 32%
        - Sans avis: 10 |||||||||| 45%
        - Très dérangeant, rédhibitoire: 5 ||||| 23%
    - De façon souhaiteriez vous pouvoir contribuer-modifier le RNB ?
        - En réalisant une contribution depuis la carto: 5 |||| 18%
        - A travers l’interface de mon logiciel métier:  5 |||| 18%
        - Via un module QGIS: 4 ||| 14%
        - Directement par API: 13 |||||||||| 46%
        - Autre : 1 | 4%

## Niveaux de contribution

Les discussions ont également porté sur la manière dont les contributions pourraient être classées en différents niveaux :

1. **Contributions certifiantes** : Ces contributions proviennent de flux administratifs qualifiés, ce qui garantit leur fiabilité. Par exemple, une commune pourrait fournir une adresse validée à travers un processus officiel.
2. **Contributions directes** : Ces contributions peuvent être faites par des professionnels qui se déplacent sur le terrain et remarquent des modifications. Les diagnostiqueurs dans le cadre de DPE, par exemple, pourraient signaler des changements lors de l'exécution de leur travail.
3. **Signalements** : Ce niveau permet aux utilisateurs, qu'ils soient professionnels ou non, de signaler des erreurs ou des inexactitudes. Cela pourrait inclure des signalements d'erreurs dans le RNB, mais nécessiterait une évaluation de la fiabilité des informations fournies.

## Volume de contributions

Un point de consensus a été atteint sur la question du volume des contributions et des signalements. Les participants ont convenu qu'il serait préférable de commencer sans limite sur les contributions afin d'encourager une participation plus large. Cependant, cela doit être accompagné d'une stratégie claire pour évaluer et traiter ces contributions afin d'éviter une surcharge d'informations non qualifiées.

## Gestion des contributions et animation de la communauté

Un des défis soulevés lors de la réunion concerne la gestion des contributions et l'animation de la communauté des utilisateurs du RNB. Il a été souligné que sans une animation active, le référentiel pourrait rapidement devenir obsolète et ne pas refléter la réalité des bâtiments sur le terrain.

La nécessité de mettre en place un système de gestion des signalements a également été discutée. Cela inclurait un processus pour traiter les informations recueillies et les transformer en contributions utiles pour le RNB. Une attention particulière a été portée sur la gestion des conflits d'interprétation, où différents contributeurs pourraient avoir des avis divergents sur la classification d'un même bâtiment. La mise en place d'un outil de médiation pour résoudre ces différends a été suggérée.

## Intégration des nouvelles constructions

Un point essentiel abordé a été l'importance d'intégrer les nouvelles constructions dans le RNB dès leur Autorisation de Droit des Sols (ADS). Il a été proposé d'impliquer les syndicats de constructeurs et d'autres acteurs du secteur pour s'assurer que les informations relatives aux nouveaux bâtiments soient rapidement et efficacement intégrées dans le référentiel.

## Échanges sur les outils et les processus

Les participants ont également discuté des outils disponibles pour faciliter les contributions et l'intégration des données. **L'utilisation d'APIs** a été proposée comme un moyen d'assurer une intégration continue et fluide des données entre le RNB et d'autres systèmes existants. L'idée est de permettre aux collectivités et aux professionnels d'accéder facilement aux données du RNB et de les mettre à jour en temps réel.

## Défis liés à la qualité des données

La réunion a mis en lumière plusieurs défis liés à la qualité des données. Il a été reconnu que les contributions provenant de différentes sources peuvent varier en qualité et en fiabilité. Pour remédier à cela, il a été suggéré d'établir des critères clairs pour évaluer la fiabilité des contributions, ainsi qu'un système de validation qui pourrait être appliqué à chaque niveau de contribution.

Quelques communes se sont portées volontaires pour tester les premières opportunités de contributions directes dans le RNB

- **Strasbourg** : L'Eurométropole propose un mécanisme de **correction massive** via une API pour rendre les données du RNB plus précises, tout en prenant en compte leur expertise locale sur le terrain.
- **Grand Orly Seine Bièvre** : Propose une collaboration via une API pour enrichir mutuellement les bases de données et améliorer la qualité des données en s'appuyant sur des relevés terrain et des prestataires locaux

# Conclusion

En conclusion, L'enjeu principal réside dans la balance entre l'ouverture des contributions à un large public tout en maintenant un contrôle de qualité strict pour éviter une surcharge de signalements incorrects.

Les discussions ont souligné l'importance d'une collaboration étroite entre les collectivités, les professionnels du bâtiment et les contributeurs afin de bâtir un référentiel robuste et utile pour tous.

 Cela inclut la nécessité d'une animation continue de la communauté, la gestion rigoureuse des contributions, et l'engagement de tous les acteurs pour faire du RNB une véritable référence nationale en matière de données bâties.
