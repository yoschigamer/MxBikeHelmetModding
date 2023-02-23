
# MxBikeHelmetModding
Make a Modded helmet in mxBike

# Files

helmet_s.edf = shadow
helmet.edf = LOD config file

# Ressources

https://docs.piboso.com/wiki/index.php?title=Main_Page
https://www.youtube.com/watch?v=JvaA2tibxi0

You can find all Tool here : https://www.mx-bikes.com/?page=downloads


```
La ligne name permet de modifier le nom de votre mod en jeu.
⚠️ n'oubliez pas de la changer ⚠️

📁 FolderOfYourMod // < Empty : Plain Axes >
 ┣ 📄 c_helmet.edf <- 
 ┣ 📄 cameras.cfg <- permet de modifier la caméra Fov, Position, etc.
 ┣ 📄 YourMask.ini <- set le nom de votre mod.
 ┣ 📄 gfx.cfg
 ┣ 📄 helmet.edf <- votre model après conversion de fbx en edf
 ┣ 📄 helmet.fbx 
 ┣ 📄 helmet.hrc <- permet de gérer les parametre de LOD [Exemple](###Code-helmet.hrc)
 ┣ 📄 helmet_s.edf
 ┗ 📄 votre Model 3d
 ```
<code>
La ligne name permet de modifier le nom de votre mod en jeu.
⚠️ n'oubliez pas de la changer ⚠️

📁 FolderOfYourMod // < Empty : Plain Axes >
 ┣ 📄 c_helmet.edf <- 
 ┣ 📄 cameras.cfg <- permet de modifier la caméra Fov, Position, etc.
 ┣ 📄 YourMask.ini <- set le nom de votre mod.
 ┣ 📄 gfx.cfg
 ┣ 📄 helmet.edf <- votre model après conversion de fbx en edf
 ┣ 📄 helmet.fbx 
 ┣ 📄 helmet.hrc <- permet de gérer les parametre de LOD [Exemple](###Code-helmet.hrc)
 ┣ 📄 helmet_s.edf
 ┗ 📄 votre Model 3d
</code>
```
📁 Export // < Empty : Plain Axes >
 ┣ 📄 export.ini <- Export Config File
 ┗ 📄 model.fbx
```
```
Blender Tree
votre arborescence dans votre éditeur (Blender) doit avoir cette disposition.
⚠️ Tous les élements hors de l'élement helmet ne seront pas pris en compte. ⚠️

🔳 helmet // < Empty : Plain Axes >
 ┗ 🔻 votre Model 3d
 ```
 
### Code helmet.hrc
``` 
level0
{
	scene = helmet.edf
	name = helmetc
	switch = 0 // valeur en mètre
} // si on dépasse les 80 mètre charger la version C du casque
 ```
