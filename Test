Pour se familiariser avec le rôle d’analyste SOC, je vais prendre en main Nessus, un scanner de vulnérabilités de réseau.

Dans le cadre de ce projet, j’aurai besoin : d’une machine virtuelle, de Nessus et d'une image Windows .iso.

J’ai choisi d’utiliser VirtualBox, mais VMWare aurait très bien pu faire le travail. Je crée une machine Windows sur VirtualBox. Après avoir effectué le setup, je dois faire quelques réglages préalables pour pouvoir m’amuser avec Nessus.

Je vais rendre ma machine volontairement vulnérable pour que Nessus puisse détecter différentes vulnérabilités. Je commence par mettre en pause les mises à jour dans Windows Update. Windows permet de suspendre les mises à jour pendant 7 jours, mais on peut augmenter cette période dans les paramètres avancés de cette section.

![Updates paused](https://github.com/user-attachments/assets/ebd8e844-c4de-4ab1-9cb4-66369737c031)

Ensuite, je vais enlever les mises à jour déjà installées. Je vais dans la section pour voir l’historique des mises à jour et clique sur “Désinstaller”.

![Enlever les màj](https://github.com/user-attachments/assets/ae28fd09-a76a-4c95-ace3-5e6863322058)

Théoriquement, il ne devrait rester que ces mises à jour impossibles à enlever.

![Choisir les màj à enlever](https://github.com/user-attachments/assets/2c6792e9-5288-4783-bba8-5c73b52875ab)

Après m’être occupé de cela, je dois m’occuper du Pare-feu Windows Defender. Je vais dans les paramètres avancés et sélectionne la section “Propriétés”.
![Windows defender advanced settings into properties](https://github.com/user-attachments/assets/89491792-d2c0-4327-b479-d9e1b956ea6f)

Je vais mettre l’état de tous les profils sur “Désactivé”.

![All profiles to off](https://github.com/user-attachments/assets/f6a685b8-3bda-43f3-af34-82e1079e588d)

La dernière étape est de configurer le mode d’accès réseau de VirtualBox sur "Réseau privé hôte", d’une part pour se protéger et d’autre part pour pouvoir utiliser Nessus pleinement sur notre machine.

![VB Nessus Network](https://github.com/user-attachments/assets/a5ab0922-6a19-4f6e-bf8d-2c4794ba47d8)

Dernière étape, vérifier qu’on est accessible. J’utilise “ipconfig” sur le Terminal pour obtenir mon adresse IP et je ping ma propre adresse pour vérifier que je suis disponible.
![Verification que tout est en place](https://github.com/user-attachments/assets/b8932859-98ba-470c-88fa-8c8abba30e9b)

Je crée un compte Nessus et fais les installations nécessaires. Une fois cela fait, je crée un scan en entrant mon adresse IP. Le scan prend quelques minutes. Une fois le scan terminé, j’obtiens une interface comme celle-ci.
![Scan de base](https://github.com/user-attachments/assets/729b8aa5-c341-4a98-a66e-27131b2ad055)

En cliquant sur une des vulnérabilités, je peux voir pourquoi elle existe, les solutions pour y remédier et des ressources sur cette vulnérabilité. Je peux colmater les failles dans ma défense moi-même et vérifier avec de nouveaux scans.

![detail scan](https://github.com/user-attachments/assets/53e995cc-12a4-4329-acdd-4a4e2a07f9bc)

Je peux approfondir cette mise en situation en utilisant les Credentials, mais ce sera dans un post dédié qui arrivera plus tard.
