Projet Personnel: Détection de Plagiat avec FastText 

## Description
Ce projet permet de détecter le plagiat en comparant un texte soumis avec une base de documents. Il utilise FastText pour générer des représentations vectorielles des documents et la similarité cosinus pour mesurer leur ressemblance.

## Fonctionnalités
- Détection de similarité entre un texte soumis et des documents existants.

- Utilisation de FastText pour capturer la signification des mots.

- Gestion des variantes morphologiques des mots.

- Score de similarité basé sur la similarité cosinus.

## Technologies utilisées
Python 3.x

Gensim (FastText)

NumPy

Scikit-learn (Similarité cosinus)
 
 Installation et exécution

## Installer les dépendances
`pip install gensim numpy scikit-learn`

## Configurer la base de documents
Modifiez la variable documents dans plagiarism_detection.py pour inclure vos textes de référence :
`
documents = [
    ["le", "chat", "noir", "dort", "sur", "le", "canapé"],
    ["un", "chien", "aboie", "dans", "le", "jardin"],
    ["le", "soleil", "brille", "dans", "le", "ciel"]
]
`
## Soumettre un texte pour vérification
Ajoutez votre texte à comparer dans submitted_text :

`submitted_text = ["un", "chat", "noir", "se", "repose", "sur", "le", "canapé"]`

## Lancer la détection
`python plagiarism_detection.py`

## Exemple de sortie
Détection de plagiat : Score de similarité max = 0.85

Plagiat détecté !

(Un score élevé signifie une forte ressemblance entre le texte soumis et un document existant.)

## Améliorations possibles
- Améliorer la précision avec BERT.
-  Ajouter une interface Web pour une utilisation plus intuitive.
-  Intégrer une base de données pour stocker les documents.

