**Objectif du GT:**

**Ressources**

* [Lien vers le Mural SGPE Schéma de données bâtiment](https://app.mural.co/t/sgpe4545/m/sgpe4545/1773304547558/8c0d9359adc7b79a70fb24ad43655888a05e419d)

# **Participants**

* Adeline Ferchaud

* Alaric Defrances (Integrativ)

* Antoine Breitwiller (CSTB)

* Elisabeth Leblanc (IGN)

* Erwan Lefeuvre (Lannion-Trégor Communauté)

* Félix Veith (RNB)

* Florent Vanhoutte (Compiègne)

* Frédéric Chauvin

* Frédérique Williams (IGN, BAN)

* Inès Chaïbi (RNB, organisatrice de la réunion)

* Jean-Luc Acquitter (IGN, chargé de déploiement BAN)

* Jérémie Le Jollec (IGN)

* Julien Petit (Data ES, recensement des équipements sportifs)

* Lara Alberge (DGALN)

* Loïc Rebours (Enedis)

* Ludovic Gouëffon (Orléans Métropole)

* Marc Grossouvre (URBS)

* Mathieu Thorel (CSTB)

* Maël Reboux (Rennes Métropole, AITF, GT Adresse)

* Nathalie Orlhac (CCR)

* Olivier Aguerre (BUSDES)

* Olivier Lefebvre (Insee)

* Pascal Vigneaud

* Pasquale Sonaglia (Direction de l'Immobilier de l'État)

* Patrice Garcia

* Pélagie Lebrun (Direction de l'Immobilier de l'État)

* Pierre Laulier (Secrétaire général du CNIG)

* Régis Haubourg (CSTB/BDNB)

* Rémi Beaurain (Géo Vendée)

* Reynald Martinez (Ville du Havre, Chef du secteur Patrimoine)

* Sébastien Wehrle (Eurométropole de Strasbourg)

* Sofiane Kriat (IGN)

* Tessa Pierre-Joseph (Direction de l'Immobilier de l'État)

* Thierry Lallemand (IGN)

* Véronique Fayard (DGFiP, Bureau du Cadastre)

* Virginie Desvigne (Ville de Grenoble)

* Yolande Chavane (SGPE, Pôle numérique et données)

# Prochaines actions

* Le SGPE partagera une nouvelle version du schéma de données suite à ce GT ainsi que les modalités de prises en compte de ces retours et prochaines étapes.

* Le RNB va proposer un GT sur les retours collectés concernant les règles de gouvernance proposées.

# Présentation de cadrage (SGPE)

Yolande Chavane (SGPE) a ouvert la réunion en présentant le contexte institutionnel. Le comité stratégique "Numérique et données pour la planification écologique", co-présidé par le SGPE et la DINUM, a priorisé en décembre le chantier de structuration de la donnée bâtiment autour du RNB. Cette priorisation se traduit concrètement par un plan de convergence piloté avec la DHUP et la DGFIP, des points hebdomadaires de suivi, et des échéances de restitution (comité stratégique du 14 avril, puis juin-juillet). Le plan d'urbanisation technique prévoit deux schémas de données distincts : un de contextualisation (positionner le bâtiment dans son environnement) et un de description (caractéristiques physiques du bâtiment). L'approche revendiquée est celle des "briques de Lego" : fabriquer d'abord les briques (identifiants, liens entre entités), les assembler ensuite pour répondre aux cas d'usage. L'intention est de viser un schéma simple et réutilisable, quitte à faire des coupes, plutôt qu'un schéma exhaustif mais inutilisable.

AJOUTER LIEN VERS SLIDES SGPE dès que disponible

# Vers un schéma de donnée bâti

*Temps d'échange et de partage de proposition* autour d'une proposition  du SGPE et de quelques propositions de schémas reçues en amont du GT ([Mural](https://app.mural.co/t/sgpe4545/m/sgpe4545/1773304547558/8c0d9359adc7b79a70fb24ad43655888a05e419d))

### Le consensus central : prioriser les données socle et procéder par cercles concentriques

A plusieurs reprises, est ressorti l'importance d'un premier niveau de données socles, permettant l'identification des différents objets et permettant la circulation de la données bâtimentaire. Une approche pragmatique visant à aller au minimum et au plus simple est un préalable à l'utilisation et à la circulation.

**Le premier cercle : les pivots d'interopérabilité.** Le cœur du travail, c'est le référentiel national des bâtiments (RNB) et ses relations avec les autres référentiels socles — adresse (BAN), parcelle (cadastre), locaux (RIAL), commune, copropriété. L'enjeu est d'organiser les pivots d'interopérabilité entre ces objets, essentiellement une multi-indexation par identifiants partagés. C'est ce socle minimal qui permet la circulation des données entre systèmes d'information. Si on arrive déjà à cette double, triple, quadruple indexation partagée entre bases, c'est un acquis considérable et c'est la priorité. Il faut d'abord aller sur ce "core" et s'éviter dans un premier temps le long travail, qu'il ne faut pas négliger mais qui viendra après, de définition commune de chaque attribut.

Cette priorisation a été appuyée de plusieurs façons complémentaires au fil des échanges. La présentation initiale du schéma de contextualisation a fait apparaître de nombreux attributs (nature du bâtiment, nombre d'étages, hauteur, surface, type de chauffage, occupants, revenus…), et plusieurs participants ont alerté sur le risque de vouloir tout traiter d'un coup. Le retour d'expérience est clair : à vouloir couvrir trop de cas d'usage dans un seul schéma, on produit quelque chose d'inutilisable. Mieux vaut un socle minimal de liens entre entités, effectivement implémenté et utilisé, qu'un modèle complet sur le papier mais que personne n'adopte.

La convergence DATA-BIM est venue renforcer cette conviction : les standards descriptifs détaillés (IFC, CityGML) ne sont pas adaptés à l'échelle nationale et aux usages décisionnels grande masse. Ce qui permet réellement l'interopérabilité entre systèmes, ce n'est pas l'alignement des modèles de données métier — c'est le pivot commun par l'identifiant bâtiment/logement. C'est aussi ce que montre l'expérience du système d'information sur l'eau, cité en référence : on ne commence pas par unifier les modèles métiers, on commence par normaliser les identifiants et les liens, puis on délègue la normalisation détaillée à des missions spécialisées.

Il a aussi été souligné qu'on ne peut pas concevoir un vrai modèle de données d'échange pour les données métiers dans le cadre de cet exercice, et que dans tous les cas il faudra des implémentations de référence pour se confronter à la réalité des données. Le schéma proposé doit servir de cadre informationnel pour que les nouveaux services numériques soient interopérables dès leur création, et que les SI existants puissent se raccrocher aux identifiants partagés — pas de norme contraignante exhaustive.

**Le second cercle : les données métiers.** Viennent ensuite les relations vers les bases métiers : consommation d'eau potable, données énergétiques (points de livraison), rénovation (ANAH), construction neuve (RE2020), santé, équipements sportifs, etc. Chacune de ces thématiques nécessite de raccrocher un objet métier (point de livraison, DPE, dossier d'aide…) à des identifiants du socle de référence, tout en identifiant les producteurs et responsables de la difuciosn de ces données métiers.

On peut lister ces thématiques d'intérêt à ce stade, mais leur modélisation détaillée relève de travaux ultérieurs, portés par les écosystèmes d'acteurs concernés. Des schémas complémentaires pourront être développés par domaine, avec toujours le principe de ne pas être trop ambitieux et de rester raccroché au socle commun.

### Gouvernance de la donnée

C'est un sujet qui a traversé une bonne partie des échanges et sur lequel plusieurs participants ont insisté :

**La frontière entre données socles et données métiers.** Une distinction structurante a émergé : celle entre les données socles qu'on veut maîtriser et corriger collectivement, et les données métiers qui restent à la main de chaque producteur. Aujourd'hui, quand un utilisateur détecte une erreur et dispose de meilleures sources, il peut contribuer au RNB qui fonctionne aujourd'hui en contribution ouverte, mais pour d'autres données (fiscales notamment), la modification reste strictement à la main du producteur. Il faut trouver le bon compromis entre un niveau d'ouverture large permettant de nombreuses contributions, et un mode trop restreint peser trop de charge sur les services publics.

**La gestion des identifiants.** La question de la stabilité et de la gouvernance des identifiants a été soulevée, notamment par la Direction de l'Immobilier de l'État qui a besoin que les identifiants RNB ne changent pas constamment pour assurer le lien avec ses propres SI. Des travaux sont en cours pour traiter ce sujet. Plus largement, il a été demandé qu'on documente clairement les règles d'attribution, de modification et de cycle de vie des identifiants structurants, à l'image de ce qui existe pour les référentiels de personnes physiques.\
Le schéma suivant illustre le cycle de vie actuelle pour les bâtiments au sein du RNB : <https://rnb-fr.gitbook.io/documentation/cycle-de-vie-de-la-donnee>

**La qualité par l'usage.** L'idée a été avancée que la qualité des données augmente naturellement quand elles sont effectivement utilisées au quotidien par les services — ce qui pose ensuite la question de la gouvernance des corrections : quand une erreur est détectée, qui valide, qui corrige, selon quelle procédure ? Pour chaque type de données, les mécaniques risquent d'être spécifiques, avec des personnes différentes qui valident ou invalident.

**Protection des données et acceptabilité.** Le croisement de données personnelles (revenus, composition des ménages, occupants) a soulevé des questions d'acceptabilité citoyenne. Il a été rappelé que le schéma de données n'est pas un système d'information centralisé, mais une carte des liens entre données existantes.

### Autres sujets de discussion notables

**Schéma vs standard.** Il a été rappelé qu'un schéma de données seul ne suffit pas à assurer l'interopérabilité : il faut aussi les règles de remplissage (valeurs possibles, définitions des champs). C'est la différence entre un schéma et un véritable standard de données. Le travail commencera par le schéma, mais devra évoluer assez rapidement vers un standard complet.
