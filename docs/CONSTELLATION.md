# La constellation Actigence / The Actigence constellation

[← Présentation GitHub / GitHub profile](../profile/README.md)

Actigence relie le conseil, les outils de travail et leurs fondations logicielles. Cette carte distingue les parcours d’usage des intégrations techniques : une activité peut mobiliser plusieurs services sans qu’ils échangent automatiquement leurs données.

## Choisir son point d’entrée

| Besoin | Service | Relation avec la constellation |
| :--- | :--- | :--- |
| Accompagner une transformation | [Actigence](https://actigence.eu) | Présente le conseil, les mandats et la façon de travailler. |
| Piloter un portefeuille ou un projet | [Hub](https://hub.actigence.eu) · [PPM](https://ppm.actigence.eu) | Le Hub donne accès à ses modules métiers ; PPM renvoie vers ce point d’entrée. |
| Recueillir des informations | [Forms](https://forms.actigence.eu) | Formulaires et réponses ; diffusion par liens courts. |
| Envoyer un dossier ou un livrable | [Share](https://share.actigence.eu) | Transferts de fichiers ; liens de téléchargement produits avec Links. |
| Animer une présentation | [Interact](https://interact.actigence.eu) | Participation en direct ; liens persistants et QR codes via Links. |
| Retrouver et gérer un lien partagé | [Links](https://links.actigence.eu) | Interface de gestion du service **amc.tf**, commun à Forms, Share et Interact. |
| Illustrer un support | [Stock](https://stock.actigence.eu) | Recherche, variantes et téléchargement des fichiers originaux. Leur réutilisation dans un support est un parcours d’usage. |
| Évaluer la charge d’une équipe qualité | [Capacity](https://capacity.actigence.eu) | Simulation agrégée, scénarios et projections hebdomadaires ; application distincte du module de capacité industrielle du Hub. |
| Apprendre avec des quiz | [Academy](https://lms.actigence.eu) | Application de quiz et d’apprentissage, avec accès selon les droits accordés. |
| Organiser une bibliothèque de films | [Movies](https://movies.actigence.eu) | Identification, classement et audit de médias ; autre usage des fondations d’interface communes. |
| Obtenir de l’aide | [Helpdesk](https://help.actigence.eu/helpdesk) | Point de support ; Forms propose aussi une entrée contextualisée pour son application. |

## Trois parcours concrets

**Recueillir et transmettre.** Créer un formulaire dans Forms, diffuser son lien court, puis envoyer les fichiers utiles avec Share. Links donne à chaque ressource une adresse courte. Les réponses et les fichiers restent dans leurs applications respectives.

**Préparer et animer.** Choisir une illustration dans Stock, l’intégrer à sa présentation, puis ouvrir une session dans Interact. Son lien **amc.tf** et son QR code permettent au public de rejoindre la session. Ce parcours associe les outils ; il ne suppose pas de connecteur automatique entre Stock et Interact.

**Piloter et comprendre.** Utiliser les modules du Hub pour la gestion métier, ou Capacity pour une simulation de charge qualité. En cas de besoin, rejoindre Helpdesk. Les administrateurs des applications instrumentées consultent les événements dans la console Audit.

## Les intégrations et fondations

| Fondation | Rôle | Portée |
| :--- | :--- | :--- |
| **Links / amc.tf** | Liens courts de formulaires, de téléchargements et de participation. | Service partagé par Forms, Share et Interact ; la destination conserve ses propres règles d’accès et de validité. |
| **Theme + UI** | Couleurs, fontes, icônes, préférences d’apparence et composants React. | Fondations réutilisées notamment par Forms, Stock et Movies. Les préférences locales ne se synchronisent pas entre domaines du seul fait de partager une bibliothèque. |
| **Core + Hub** | Paquets de plateforme, contrats de modules, catalogue et navigation métier. | Socle des modules du Hub. Le Hub n’est pas un annuaire exhaustif de tous les services. |
| **[SSO](https://auth.actigence.eu)** | Expérience de connexion Actigence sur Authentik. | Services intégrés à Authentik ; connexion commune et autorisations propres à chaque application. |
| **Logger + [Audit](https://log.actigence.eu)** | Journaux structurés, SDK et consultation d’événements. | Applications instrumentées ; console réservée aux administrateurs autorisés. |

## Code, accès et origine

Le [catalogue GitHub](https://github.com/orgs/Actigence-Code/repositories) affiche les dépôts accessibles au visiteur. Les descriptions indiquent le rôle de chaque projet, ses connexions et son stade de développement. Cette page ne modifie ni l’accès aux applications ni la visibilité des dépôts.

Les intégrations conservent leur filiation : **Interact / Claper**, **Share / Plik**, **Links / Shlink**, **SSO / Authentik** et **Analytics / Plausible**. Le [fork public d’Analytics](https://github.com/Actigence-Code/actigence-analytics) est présenté par son dépôt ; son origine et sa licence restent celles documentées dans ce projet.

## English

Actigence connects consulting, working tools and their software foundations. The directory above lists service entry points; access depends on each application's permissions.

Three practical journeys illustrate the relationships: **collect and share** with Forms, Links and Share; **prepare and engage** with Stock and Interact; **plan and understand** with Hub, Capacity, Helpdesk and administrator Audit. Stock artwork is downloaded and reused by the user; this is a working journey, not an automatic Stock-to-Interact integration.

Forms, Share and Interact use the **amc.tf** short-link service. **Theme and UI** provide shared interface foundations. **Core and Hub** provide platform contracts and business-module navigation. **Authentik SSO** handles sign-in for integrated applications. **Logger and Audit** provide structured events for instrumented applications. Applications retain their own data, permissions and business rules.

Capacity's quality-team simulation is distinct from Hub's manufacturing-capacity module. Academy currently focuses on quizzes. Repository descriptions identify prototypes and current integration scope. The [repository catalogue](https://github.com/orgs/Actigence-Code/repositories) respects existing repository visibility and upstream licensing.
