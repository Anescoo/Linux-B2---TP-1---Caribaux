# Remonté d'un poste Windows 10 dans l'inventaire GLPI
---
![](Img/Windows-Server-Logo.png)

---

#### Installation de Fusion Inventory Agent

- Tout d'abord rendez-vous sur la machine virtuelle **windows 10** que vous avez précédemment installé :

![](Img/winpost4.PNG)

- Ensuite aller sur navigateur internet : google, mozilla, internet explorer, etc... Ici ce sera **Microsoft Edge** et télécharger le logiciel **Fusion Inventory Agent**.

![](Img/win1.PNG)

- On va d'abord configurer l'application.

![](Img/win2.PNG)

- On va définir un chemin d'installation :

![](Img/win3.PNG)

- On va ensuite aller chercher le lien d'accès à fusion inventory dans GLPI :

```
http://192.168.47.135/glpi/plugins/fusioninventory/
```

![](Img/win4.PNG)

- Après la configuration l'installation s'initialise :

![](Img/win5.PNG)

- Il faut ensuite aller sur le navigateur et saisir :

```
localhost:62354
```

et cliquer sur **Force an Inventory**

![](Img/win6.PNG)

- On peut remarquer que la manipulation a fonctionné :

![](Img/fusioninvage.PNG)

- Direction **GLPI**. Aller dans le menu **Parc** → **Ordinateurs**, cette interface devrait apparaitre :

![](Img/postewin.PNG)

- On peut voir sur la deuxième ligne le nom de ma machine **DESKTOP-72874UA**, le fabricant est **Vmware** (logiciel pour machine virtuelle), et le système d'exploitation est **Windows**
- La remontée du poste Windows 10 dans l'inventaire GLPI grâce à la manipulation sur la VM Windows avec **Fusion Inventory Agent** à effectivement été concluante.