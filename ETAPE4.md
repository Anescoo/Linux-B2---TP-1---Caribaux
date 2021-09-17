# Installation de Fusion Inventory
---

**C'est quoi Fusion Inventory ?**

Fusion Inventory est un logiciel servant à l'inventaire et la maintenance d'un parc informatique à l'aide d'autres logiciels de ce type tels que GLPI. Il permet d'effectuer l'inventaire matériel et logiciel.

## Installez et configurez de Fusion Inventory

- Tout d'abord il faut mettre à jour le système avec :

```
apt-get update && apt-get upgrade
```

- Ensuite on retourne dans le répertoire des sources et on télécharge le plugin **Fusion Inventory** avec un lien :

```
cd /usr/src
```

```
wget https://github.com/fusioninventory/fusioninventory-for-glpi/releases/download/glpi9.5%2B3.0/fusioninventory-9.5+3.0.tar.bz2
```
*(on va télécharger le plugin grâce la commande **wget** avec le lien)*

```
tar xfvj fusioninventory-9.5+3.0.tar.bz2 -C /var/www/html/glpi/plugins
``` 

*(on va extraire les données du téléchargement pour les transférer dans le dossier plugins en suivant ce chemin)*

- On va ensuite attribuer les droits d'accès au serveur web :

```
chown -R www-data /var/www/html/glpi/plugins
```

- Ensuite il n'y a plus qu'a finaliser l'installation sur l'interface web, tout d'abord il faut se reconnecter à **glpi**:
![](Img/glpiconnect.PNG)

- Une fois connecté, on va dans la rubrique suivante : **Configuration** → **Plugins** :
![](Img/fusinvinstall.PNG)

- Prochaine étape on devrait voir apparaitre la fenêtre suivante, il suffira de cliquer sur "**Installer**" le plugin depuis la ligne correspondante et ensuite l'activer avec le "verrou" rouge qui passera au vert : 
![](Img/fusinvinstall2.PNG)

- Voici ce que cela donne au final, félicitation **Fusion Inventory** est installé et prêt à l'emploie :
![](Img/fusioninventory.PNG)

>--- 
- Aperçu de l'interface **Fusion Inventory** :
![](Img/fusinvinterf.PNG)

---

[IV - 1 | page suivante](https://github.com/Anescoo/Linux-B2-TP1/blob/main/ETAPE6.md) >