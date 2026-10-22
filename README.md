# blog.pypinho.fr

Site statique servi par Coolify (nginx) sur le VPS. **Chaque push sur `main` redéploie le site automatiquement.**

## Structure

```
index.html              page d'accueil, liste des articles
<slug>/index.html       un article = un dossier, servi sur blog.pypinho.fr/<slug>/
```

## Publier un article (depuis n'importe quelle interface Claude)

1. Créer `<slug>/index.html` : une page HTML autonome (doctype, head, styles inline).
   Lien de retour en haut : `<a href="/">← blog.pypinho.fr</a>`.
2. Ajouter un `<li>` en tête de la liste `.posts` dans `index.html` (date, titre, une phrase).
3. Commit + push sur `main`. Le site est à jour une minute plus tard.

Slugs en minuscules, sans accents, mots séparés par des tirets.

## Articles

- `echelle-nate/` : les 7 barreaux de Nate Hagens (Frankly #162), façon Wait But Why. 22/10/2026.
