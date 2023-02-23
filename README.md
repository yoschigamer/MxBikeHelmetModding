
# MxBikeHelmetModding
Make a Modded helmet in mxBike

# Ressources

https://docs.piboso.com/wiki/index.php?title=Main_Page
readme Réalise grace à la vidéo ci dessous : https://www.youtube.com/watch?v=JvaA2tibxi0

You can find all Tool here : https://www.mx-bikes.com/?page=downloads


```
La ligne name du fichier <YourMask.ini> permet de modifier le nom de votre mod en jeu.
⚠️ n'oubliez pas de la changer ⚠️

📁 FolderOfYourMod // < Empty : Plain Axes >
 ┣ 📄 c_helmet.edf <- model.fbx après convertion.
 ┣ 📄 cameras.cfg <- permet de modifier la caméra Fov, Position, etc.
 ┣ 📄 YourMask.ini <- set le nom de votre mod.
 ┣ 📄 gfx.cfg
 ┣ 📄 helmet.edf <- votre model après conversion de fbx en edf.
 ┣ 📄 helmet.fbx 
 ┣ 📄 helmet.hrc <- parametre du LOD.
 ┗ 📄 helmet_s.edf <- paramètre des ombres.
 
📁 Export
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
 
### Script helmet.hrc
``` 
level0
{
	scene = helmet.edf
	name = helmetc
	switch = 0 // valeur en mètre
} // si on dépasse les 80 mètre charger "helmetc"
 ```

### Script export.ini
```
export.ini: [Hierarchy]
split = 1 
rotation = -70 180 90 // laissé par défaut (Recommandé)
helmet = *your path*\Export\helmet.edf // endroit ou votre fichier va ètre exporté
```
