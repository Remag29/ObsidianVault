![[Pasted image 20231013104859.png]]

La politique d’accès peut être embarquée dans les clés de déchiffrement (Key Policy Attribute-Based Encryption, KP-ABE). L’autorité génère et conserve une clé maître. Elle diffuse au service la clé publique associée. Le service utilise cette clé publique et l’ensemble des attributs calculé par le PIP pour chiffrer le message. Le chiffré est diffusé aux clients. En utilisant la clé maître et la politique donnée par le PAP, l’autorité génère une clé de déchiffrement pour chaque client. Chaque clé embarque une politique de contrôle d’accès, et ne peut déchiffrer que si le chiffré a été produit avec un ensemble d’attributs accepté par la politique embarquée dans la clé de déchiffrement. Avec KP-ABE, l’autorité impose donc la politique de contrôle d’accès, et laisse le service librement fixer les attributs dans le chiffré.

![[Pasted image 20231017133251.png]]

KP-ABE