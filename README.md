# Lancer server develop (pour moi)
hugo server --bind "0.0.0.0" -p 8083


# Structure
- data                    > contenu textuel + lien vers images
- static/assets/img       > les images que tu veux uploader
- thmes/graysx/layouts    > manipuler le html
- thmes/graysx/static     > manipuler le css

# Lancer le build
Juste faire "hugo" dans la console et le dossier public est généré

# Custom style
Dans le fichier styles.css ligne ~70 t'as un pavé ou j'ai expliqué un peu le fonctionnement. 
T'as juste à changer les valeurs hexadecimal en couleur que tu preferes pour tester des ajustements differents.
Fais pas gaffe aux noms de variables (cf teal, green...) j'ai laissé ca mais on sen fou c'est juste une variable change uniquement la valeur

Le premier bloc c'est les boutons (contact us) et les menus en haut
```css
/** btn and menu **/
--bs-custom-btn-teal: #94a164;
--bs-custom-btn-teal-hover: #50817e;
```

Ici le fond ou il y les cards
```css
/** background light for the cards / bigcards **/
--bs-custom-greenlight: #f5f3f5;
```

Et enfin les parties les plus sombre et petit truc relou a faire mais faut aussi fournir la valeur rgb de la couleur que tu choisi car le css en a besoin
```css
/** All darks backgrounds head / about section / footer **/
--bs-custom-greendark: #7957c2;
--bs-custom-greendark-rgb: 149, 177, 174;
/** RGB value of above the bs-custom-greendark **/
```