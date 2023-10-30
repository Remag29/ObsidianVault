![[Pasted image 20231013104930.png]]

La politique d’accès peut être embarquée dans le chiffré (Ciphertext Policy Attribute-Based Encryption, CP-ABE). L’autorité génère et conserve une clé maître. Elle diffuse au service la clé publique associée. Le service utilise cette clé publique et la politique donnée par le PAP pour chiffrer le message. Le chiffré est diffusé aux clients. En utilisant la clé maître et l’ensemble d’attributs calculé par le PIP, l’autorité génère une clé de déchiffrement pour chaque client. Chaque clé embarque l’ensemble d’attributs calculé par le PIP, et ne peut déchiffrer que si cet ensemble d’attributs est accepté par la politique embarquée dans le chiffré. Avec CP-ABE, l’autorité certifie donc les attributs possédés par chaque client, et laisse le service librement décider la politique de contrôle d’accès.

CP-ABE

### Résistance aux collusions
[source](https://fr.wikipedia.org/wiki/Chiffrement_par_attributs)
Un aspect essentiel de la sécurité du chiffrement par attributs est la résistance aux [collusions](https://fr.wikipedia.org/wiki/Collusion "Collusion"), c'est-à-dire que des utilisateurs ne doivent pas être capable de mettre en commun leurs clés secrètes pour déchiffrer des messages qu’aucun d’entre eux n’est capable de déchiffrer seul. Par exemple, pour le message envoyé avec la politique (A∧C)∨D, un utilisateur possédant l’attribut ***A*** et un utilisateur possédant l’attribut  ***C*** ne peuvent pas mettre en commun leurs informations pour déchiffrer le message.