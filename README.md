# Stanford University — site d'exposé d'anglais

Support de présentation pour un exposé d'anglais en binôme au collège.
Une seule page, de gros boutons par thème : pendant l'oral, on choisit un thème,
ses photos tournent toutes seules (5 secondes chacune, bouton Pause), et les
mots-clés restent lisibles de loin.

## Comment l'utiliser

- Ouvrir `index.html` dans un navigateur (double-clic suffit, même hors ligne).
- Cliquer un thème → photos en boucle + mots-clés. Boutons ◀ ▶, ⏸ Pause / ▶ Play.
- Retour : bouton « ← All topics » ou touche Échap.

## Modifier le contenu

Tout le texte est au début du `<script>` dans `index.html`, dans la liste `THEMES`.
Un thème = un bloc entre `{` et `}` : `name` (titre), `keywords` (mots-clés),
`images` (photos + crédits). Supprimer un bloc retire le thème du site.

## Ajouter des animations

Chaque thème a une ligne `animation: null`.
Remplacer `null` par une fonction qui reçoit la boîte d'affichage, par exemple :

```js
animation: function(box){ box.style.border = "6px solid gold"; }
```

Elle est lancée automatiquement à l'ouverture du thème (voir `startAnimation`
dans le code, commentaires en français).

## Sources des informations

Toutes les infos viennent de sources officielles Stanford (relevé du 21 novembre 2026) :
stanford.edu, facts.stanford.edu, financialaid.stanford.edu, studentservices.stanford.edu,
museum.stanford.edu, library.stanford.edu, admission.stanford.edu.

## Crédits photos (toutes réelles, licences libres, via Wikimedia Commons)

- Main Quad (x2) et vue depuis Hoover Tower : King of Hearts, CC BY-SA 3.0
- Palm Drive : Jawed Karim, CC BY-SA 3.0
- Hoover Tower : King of Hearts, CC BY-SA 3.0
- Memorial Church : Frank Schulenburg, CC BY-SA 4.0
- HP Garage : Oysterboy9, CC BY-SA 4.0 ; Arild Finne Nybø, CC BY-SA 2.0
- SLAC : Alfred Twu, CC0 ; Pi.1415926535, CC BY-SA 3.0
- Stanford Stadium : BrokenSphere, CC BY 3.0
- Rodin Sculpture Garden : GualdimG, CC BY-SA 4.0
