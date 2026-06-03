# **Compte Rendu GT Bâti Session 17**

**27 avril 2026**

## **Participant.e.s**

* Animateur.trice.s

  * Inès CHAïBI (RNB)

  * Felix VEITH (RNB)

* Participant.e.s

  * Acquitter Jean-Luc – IGN/RNB

  * AFONSO Filipe – Stonal

  * ANSARD Cédric – Région Hauts-de-France / Géo2France

  * BEAURAIN Rémi – GéoVendée

  * BOUDIN Antoine

  * CHAVANE Yolande – SGPE

  * CHAUVIN Frédéric. – Rennes Métropole

  * FERCHAUD Adeline – Bordeaux Métropole

  * GALLAIS Arnaud – Cerema

  * GARCIA Patrice – ARS PACA

  * GODEFROY Véronique – Orléans Métropole

  * GROSSOUVRE Marc – U.R.B.S

  * HAUBOURG Régis – CSTB

  * JASSON Guillaume – ACTEE

  * KRIAT Sofiane – IGN

  * LEFRANCOIS Paul – Integrativ

  * MAISONNAVE Mireille – Conseil départemental d’Indre-et-Loire

  * MATHIS Loïc – Métropole de Lyon

  * MONTI Romain

  * ORLHAC Nathalie – CCR

  * PAUGET MYRIAM – SIEA

  * PETIT Julien – CREPS Pays de la Loire

  * PIERRE-JOSEPH Tessa – DGFiP

  * REBOURS Loïc – Enedis

  * REBOUX Maël – Rennes Métropole

  * SAVARY Olivier – Région Hauts-de-France

  * THOREL Mathieu – CSTB

  * VANHOUTTE Florent – Compiègne et son agglomération

  * WILLIAMS Frédérique – IGN

## **Sujet du GT :**

* Établir et valider les règles de gouvernance de la donnée RNB.

## **Ressources**

* [Lien vers le support Mural]( <https://app.mural.co/t/batid0128/m/batid0128/1694501566798/81ce9afcdb7151d90115217b997ae875e46b0f84>)
- Le support mural est égaleemnt stocké [ici](CNIG/Comptes-Rendus/CR-GT-17-Support-Mural.png)

![image.png](https://docs.numerique.gouv.fr/media/a2cf9d0a-b1ed-4599-b16a-472c078f95f1/attachments/146647b8-ffc6-43e2-ad12-d3b6b19f6bd1.png)

## **Cadrage**

Rappel de la mission du RNB : **Référencer tous les bâtiments observables sur le territoire, qu'ils soient légaux ou non.**

Le RNB référence 44 millions de bâtiments, avec 380 000 éditions réalisées par 310 comptes éditeurs. Sur les 380 000 éditions, seuls 210 bâtiments ont reçus des éditions de plusieurs comptes, et le taux d'erreur mesuré est de 3 %.

**Ce GT clôture l'appel à commentaires&#x20;**&#x71;ui s'est tenu sur le Forum des géocommuns : <https://forum.geocommuns.fr/t/appel-a-commentaire-jusquau-22-avril-regles-de-gouvernance-de-la-donnee-rnb/3123> , avec :

* **295 vues de la discussion**

* **275 vues de la page des règles de gouvernance actuelles** AJOUTER PDF DE LA PAGE

## **Prochaines étapes**

* Partager les règles de gouvernance cibles basées sur les consensus actés durant le GT. Date : été 2026

* Intégrer les éléments de consensus dans la feuille de route produit du RNB. Date : T3 2026

* Creuser les options sur le système de tampons (validation de bâtiment) :

  * **Phase 1 :** tester le principe de base de tampon et tester les scénarios de conflits d'édition entre institutions . Date : été 2026.

    * expérimenter la fonction de tampon en mode ouvert et beta. Ce mode est le plus rapide et simple à mettre en place. Le code sera réutilisable quelque soit la direction prise.

    * tenir un atelier 'cas pratique' pour expérimenter les tampons ouverts uniquement aux services publics : sélectionner 2/3 cas et projeter quelle entité peut agir dessus. Participants nécessaires : DIE, administration (data ES par ex), région, département, EPCI, commune.

  * **Phase 2&#x20;**: se concerter avec le GT Bâti pour confirmer la direction à prendre concernant les tampons (utile ou non) et la gestion des droits (ouvert, fermé, hybride), en se basant sur les 2 retours d'expérience. Date : octobre 2026

  * **Phase 3&#x20;**: intégration des décisions au produit et mise à jour des règles de gouvernance. Date : fin 2026

***

## **1- Points clés des règles actuelles soumises à l'appel à commentaire**

![image.png](https://docs.numerique.gouv.fr/media/a2cf9d0a-b1ed-4599-b16a-472c078f95f1/attachments/45124097-60ce-47a9-afd7-fde8055b6022.png)

Il est rappelé qu'un bac à sable est disponible pour tester les contributions massives avant intégration en production.

***

## **2- Evolutions des règles qui font consensus**

* Renforcer l'identification avec Pro Connect et France Connect sans que ce ne soit obligatoire. Limites soulevées sur FranceConnect : peut être perçu comme trop personnel, âge minimum, accès limité.

* Pouvoir apposer un tampon 'Bâti revu et validé' visible par toutes et tous.

* Pouvoir s'abonner à un ou des bâtiments et recevoir des notifications suite à une édition, un signalement, une modification apportée par l'administrateur ou un tampon apposé.

* Analyser la pertinence et les possibilités d'évolution de gestion des imports pour qu'ils puissent modifier des bâtiment qui ont été édités. En cas de doute, toujours privilégier la source RNB. A savoir : l'IGN travaille à intégrer les modifications du RNB dans les mises à jour de la BD Topo, ce qui réduira les écarts.

* Pouvoir bannir ou bloquer des comptes d'édition, dans des cas limités et bien définis, à préciser.

* Consolider le système de back up, augmenter leur fréquence (quotidienne).

* Connaître son seuil et son nombre d'édition en tant que contributeur (sur la carte et via API). Il a été soulevé un risque de goulot d'étranglement avec ce principe de seuil.

## **3- Nouvelles pistes à étudier**

* Automatiser la détection des comportements malveillants.

  * Limitation d'adresses IP selon la localisation ou patterns.

  * Pour les mesures de protection, permettre d'ajuster en permanence les protections avec rate limiting, black listing d'url (avec pleins de règles métiers) via un portail d'API.

  * Mettre en place des algorithmes pour :

    * Détecter les modifications suspectes (ex : 1 000 éditions en 1 jour).

    * Bloquer temporairement les comptes avant validation manuelle.

* Commencer à prévoir des systèmes de validation et contrôle de qualité compatible avec le passage à l'échelle

* Badges : Idée de niveaux de confiance (ex : badge "communauté" pour les contributeurs réguliers, badge "institution" pour les collectivités).

* Pouvoir s'abonner à un périmètre géographique

* Utiliser les ADS pour mettre à jour le RNB ( construction et démolition)

***

## 4- Echanges sur les points d'arbitrage : Tampon ouvert vs institutionnel et mode de gestion de désaccords d'édition

### a- **Ouverture vs. contrôle institutionnel**

* **Débat central** :

  * **Modèle ouvert** (tout le monde peut éditer) vs. **modèle institutionnel** (seules les collectivités/administrations peuvent éditer leur patrimoine).

  * **Risques** :

    * **Modèle ouvert** : Pollution possible, manque de fiabilité pour les institutions, crainte de modification non justifiée sur son parc, crainte d'acte de malveillance.

    * **Modèle fermé** : **Découragement des contributions individuelles**. Nécessite un **engagement des institutions à maintenir à jour** le RNB (vérification annuelle). Pose la question de **qui est légitime entre institutions** (ex : commune vs. département pour un bâtiment scolaire, DIE vs EPCI etc). Perte de réactivité : amène une complexification du RNB et donc une perte de fluidité et performance. Exclusion de constatation terrain d'individus.

* **Proposition** :

  * **Expérimenter** un système ouvert avec **gardes-fous** (tampons, modération, abonnements).

  * **Principe** : **"Grand pouvoir, grande responsabilité"** → Limiter les droits si abus avérés.

  * L'expérimentation va permettre de

    * constater les comportements institutions, entreprises, bailleurs et individus

    * vérifier si les non institutionnels se concentreront sur les bâtis sans tampons

    * vérifier si des cas de conflits d'édition se présentent

    * tester la fonction tampon

    * vérifier si le tampon apporte bien une fiabilité supplémentaire de la donnée

    * vérifier si la possibilité d'avoir plusieurs tampons sur un même bâti est utilisée

### **b - Cas de conflit / désaccord sur un bâti:**

* Si un bâtiment tamponné est modifié, ne pas rendre **obligatoire le commentaire**. Crainte de commentaire vide, de frein à l'amélioration de la donnée, et trop de notification.

* **Chute du tampon** en cas de modification (pour refléter l’évolution du terrain). Le tampon reste tracé dans l'historique.

* **Possibilité de rollback** par l’administrateur en cas de désaccord persistant.

* **l'idéal serait un outil de discussion intégré** pour résoudre les désaccords (ex : forum lié au bâtiment).

### **c- Que valide un tampon :**

Faut-il tamponner **l’ensemble du bâtiment** ou **des attributs spécifiques** (ex : adresse vs. géométrie) ?

* Son état au moment du tampon.

* Pas de granularité à mettre en place (on ne tamponne pas que l'adresse ou la géométrie) cela apporterait trop de complexité, et ne correspond pas à la mission du RNB : identifier un bâti

### **d- Un tampon abonne automatiquement au bâti**

* risque de trop de notification

* laisser le choix à l'utilisateur
