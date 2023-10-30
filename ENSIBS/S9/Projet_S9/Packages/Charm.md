# Charm
[Charm GitHub](https://github.com/JHUISI/charm)
***Charm*** est utilisable via Python.
## Installation
***Charm*** possède 3 dépendances :
- [GMP 5.x](http://gmplib.org/)
- [PBC](http://crypto.stanford.edu/pbc/download.html)
- [OPENSSL](http://www.openssl.org/source/)

Il faut donc les installées avant.
Pour cela, on prossède de la même manière pour les 3.
- On commence par télécharger l'archive
- Décompresse
- Exécute le `./configuration`
- Exécuter `make` dans le dossier en question
- Exécuter `sudo make install` pour installer le logicielle

Après avoir fait cela pour les 3 dépendances, on peut venir faire la même chose pour ***Charm*** cette fois ci :
```bash
./configuration
make
sudo make install
```

Après cela, ***Charm*** est normalement correctement installé.

## Utilisation
Pour l'utilisation de Charm, on se base sur l'approche du repository suivant : [ABE with Charm](https://github.com/sagrawal87/ABE)

Pour utiliser ***Charm*** dans le but de faire une infrastructure de *CP-ABE*, on peut commencer pas créer un objet de ce type :
```python
# instantiate a bilinear pairing map
pairing_group = PairingGroup('MNT224')  

# AC17 CP-ABE under DLIN (2-linear)
cpabe = AC17CPABE(pairing_group, 2)
```

`cpabe` est donc l'objet qui va nous permettre d'effectuer toutes les actions que l'on veut (Créer des clés, chiffrer, déchiffrer, etc...)

### Génération des clés PK et MK
On peut venir créer notre jeu de clés.
`pk` --> Clés Public
`msk` --> Clés Maitre

```python
# run the set up
(pk, msk) = cpabe.setup()
```

### Génération d'un clés SK
Les clés `SK` sont destiné aux utilisateurs. Dans le cas de *CP-ABE*, ce sont elles qui contiennent les attributs qui sont propres à l'utilisateurs.
On peut venir créer une `sk` avec la commande suivante :
```python
# generate a key
attr_list = ['ONE', 'TWO', 'THREE']
key = cpabe.keygen(pk, msk, attr_list)
```

On a par exemple ici une clés qui contient les attributs `ONE`, `TWO` et `THREE`.