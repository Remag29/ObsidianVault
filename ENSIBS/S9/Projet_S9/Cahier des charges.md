# Rappel du contexte et de la problématique

Dans le domaine militaire, le partage de données sur des réseaux privés revêt une importance cruciale pour assurer la sécurité nationale et la prise de décisions éclairées.
Les forces armées modernes fonctionnent de manière de plus en plus interconnectée, avec des données provenant de diverses sources, telles que satellites, drones, capteurs terrestres et informations provenant de l'intelligence humaine. Ces données, bien que très sensibles, alimentent les opérations militaires, la surveillance des menaces et les efforts de renseignement. 
Le volume considérable de ces données, générées en temps réel, présente un défi de gestion complexe. La capacité de partager efficacement ces informations au sein de réseaux privés sécurisés permet aux commandants et aux analystes de disposer d'une vue d'ensemble précise, favorisant ainsi une meilleure coordination des opérations et la réponse rapide aux menaces émergentes, tout en garantissant la protection des données sensibles contre les adversaires potentiels.

Cependant, malgré l'importance des réseaux privés dans le domaine militaire, il est parfois nécessaire d'utiliser des réseaux publics pour transmettre d'énormes volumes de données. Les réseaux publics offrent une plus grande capacité de transmission, permettant ainsi de partager des informations à l'échelle mondiale en temps réel. Toutefois, cette utilisation nécessite des mesures de sécurité et de chiffrement pour protéger les données militaires sensibles contre d'éventuelles menaces.

> **Dans un contexte de conflit militaire, peut-on envisager ABE comme une solution viable pour assurer la sécurité des données sensibles et maintenir l’intégrité du “droit d’en connaître” lors de communications sur des réseaux publics ?**


# Etude bibliographique sur les travaux sur le sujet

Les études bibliographiques mis à notre disposition dans la proposition de projet met en lumière des technologies très intéressantes.

Dans un premier temps, nous avons la citation du concept de ***DCS***.
Le ***DCS***, ou ***Data-Centric Security*** (Sécurité centrée sur les données), est une approche de la sécurité informatique qui met l'accent sur la protection des données elles-mêmes plutôt que sur la sécurité des périmètres ou des points d'accès. L'objectif principal du DCS est de renforcer la sécurité des données, en mettant l'accent sur leur importance et leur confidentialité.

Parmi les deux papier de recherche cité, on relève la présence constante de la technique ***ABE***.
L'***ABE***, ou ***Attributed-Based Encryption*** (Chiffrement basé sur les attributs), est une technique de chiffrement qui permet de contrôler l'accès aux données en fonction des attributs des utilisateurs. Au lieu de se baser sur des identités spécifiques, l'ABE autorise ou restreint l'accès en fonction de critères prédéfinis, tels que l'appartenance à un groupe, le rôle, ou d'autres caractéristiques d'un utilisateur.

Le lien entre l'ABE et le DCS (Data-Centric Security) réside dans le fait que l'ABE est l'une des techniques utilisées pour mettre en œuvre une approche de sécurité centrée sur les données. En utilisant l'ABE, les données peuvent être chiffrées de manière à ce que seuls les utilisateurs possédant les attributs appropriés puissent les déchiffrer. Cette approche permet un contrôle fin de l'accès aux données en fonction des besoins de sécurité et de confidentialité, renforçant ainsi la protection des données sensibles dans le cadre du DCS. En combinant l'ABE avec d'autres mesures de sécurité, le DCS peut être mis en œuvre de manière plus efficace pour garantir la sécurité des données tout au long de leur cycle de vie, que ce soit lors de leur stockage, de leur partage ou de leur utilisation.

# Description de l'objectif visé et sa différentiation avec les travaux existant

L'objectif principal de cette étude est d'abord de réaliser une revue exhaustive de la recherche sur les concepts du Data-Centric Security et de l'Attribute-Based Encryption. Le but est de se familiariser avec ces domaines de recherche relativement récents pour en saisir les principes fondamentaux.

Ensuite, la démarche centrale consiste à mettre en place une Proof of Concept (POC) simulant "Mon Espace Santé" en appliquant une politique de sécurité basée sur l'ABE. L'objectif principal de cette POC est d'assurer la sécurité des données médicales tout en respectant le principe du "droit d'en connaître". Il faudra donc déterminer avec précision les attributs pertinents pour les utilisateurs et les données. Cette POC permettra également d'identifier les éventuels problèmes de sécurité ou d'intégration susceptibles de découler de l'utilisation de l'ABE.

Cette étude vise à faire progresser la compréhension du fonctionnement d'ABE tout en évaluant sa fiabilité et son applicabilité dans un contexte spécifique.

