# World Discovery

## Organisation du projet

### Front end

#### Public

**Header** 
- Nav bar : Logo, nom du site, Home, contact (qui renvoit au footer)

**Footer**
- Contact 
- Réseaux sociaux

**Page d'acceuil**
- Caroussel d'acceuil avec des photos des differentes destinations 
- Paragraphe pour presenter le but du site etcc
- 6 cards : une pour chaque continent avec une photo pour chacune
- A la fin on peut mettre une map avec des pins en rouge pour les endroits où on est partis 

**Page continent : après avoir cliqué sur une card**
- Des cards avec les différents pays 
- Un endroit pour rechercher plus facilement les destinations
- Map zommée sur le continent avec les pins en rouge pour les endroit où on est partis

**Page destination**
1. Général :
- Durée du séjour
- Période de l'année 
- Combien de personne 
- Contexte (pour les vacances, pour un stage, etc...)

2. Itinéraire
- Description du voyage idéalement jour par jour mais pas nécessaire (avec illustrations,tips...)
- Catégories (Les activités marquantes, les meilleurs spots, les meilleurs resto/cafés/fast-food)

3. Budget 
- Budget approximatif des activités + forfait téléphonique + bouffe en général (en précisant notre type de voyage : économique, luxe...)
- Prix du billet d'avion
- Prix des transports là bas...
 
4. Catégorie matos photo
5. Conseils + conclusion de ce qu'on en a pensé


#### Administrateur (TDB)

**Acceuil TDB**

Navigation disponible vers :
- Gestion des destinations

**Gestion des destinations**

Affichage de toutes les destinations déjà publiées sous forme arborescente : continent -> pays
Possibilité de :
- Créer une nouvelle destination
- Modifier une destination déjà existante

**Créer / modifier une destination**

Form :
- Nom du pays
- Continent
- Pour chaque catégorie : possibilité de choisir entre une image, un paragraphe ou les deux


### Back end

#### Base de données

**Organisation des fichiers**
- files
    - continent
        - pays
            - caroussel
                - picture0
                - picture1
                - ...
            - cover.(jpg|png)
            - content.json

**Tables**
- Destinations :
    - Pays (clé primaire)
    - Continent associé
    - Budget total (pour filtrer par budget)
    - Nombre de personnes (pour filtrer par budget)
