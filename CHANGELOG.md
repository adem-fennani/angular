# Changelog

Toutes les modifications notables de ce projet seront documentées dans ce fichier.

---

## Workshop 2 - Manipulation des Composants
**Date : 02/02/2026**

### Ajouté
- **Composant Header** (`app-header`) - En-tête de l'application
- **Composant Footer** (`app-footer`) - Pied de page de l'application
- **Composant ListSuggestion** (`app-list-suggestion`) - Affichage de la liste des suggestions
- **Interface Suggestion** - Modèle de données pour les suggestions avec les propriétés :
  - `id` : Identifiant unique
  - `title` : Titre de la suggestion
  - `description` : Description détaillée
  - `category` : Catégorie (Événements, Technologie, Ressources Humaines)
  - `date` : Date de création
  - `status` : Statut (acceptee, refusee, en_attente)
  - `nbLikes` : Nombre de likes

### Fonctionnalités
- **Interpolation** (`{{ }}`) - Affichage dynamique des données
- **Property Binding** (`[property]`) - Liaison de propriétés
- **Event Binding** (`(event)`) - Gestion des événements (click)
- **Two-way Binding** (`[(ngModel)]`) - Liaison bidirectionnelle pour la recherche
- **Directive NgFor** (`*ngFor`) - Boucle pour afficher la liste des suggestions
- **Directive NgIf** (`*ngIf`) - Affichage conditionnel des boutons

### Interactions utilisateur
- Bouton **"Like"** - Incrémente le nombre de likes d'une suggestion
- Bouton **"Ajouter aux favoris"** - Ajoute une suggestion à la liste des favoris
- Les boutons sont masqués pour les suggestions avec le statut "refusee"
- **Barre de recherche** - Filtre les suggestions par titre et catégorie

