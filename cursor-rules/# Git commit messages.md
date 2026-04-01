---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Messages de validation Git

Appliquez toujours cette règle. Lorsque vous rédigez ou générez un message de validation Git (par exemple dans la zone de validation du contrôle Source ou lorsque vous y êtes invité dans la conversation de l’agent), suivez ce format.

## Objet (première ligne uniquement)

- Environ **50 caractères ou moins**.
- Résumez le changement d’humeur **impérative** (par exemple, « Ajouter... », « Corriger... », « Refactoriser... »).

## Ligne vide

Laissez une **ligne vide** après l’objet avant le corps.

## Corps (description détaillée)

- Placez des lignes à environ 72 caractères **(y compris le préfixe et l’espace des puces).**
- Utilisez **puces** pour l’explication. Chaque puce doit commencer par exactement l’une des valeurs suivantes :
   - **📖** — à utiliser lorsque la modification **ajoute** quelque chose de nouveau : nouveaux fichiers, nouvelles sections, nouvelles fonctionnalités, nouveaux en-têtes, nouvelles lignes ou autre contenu nouveau.
   - **✏️** — utiliser lorsque la modification **modifie** travail existant : modification de lignes existantes, mise à jour de sections existantes, refactorisation de code existant ou modification du contenu actuel.

Appliquez du **📖** ou du **✏️** à chaque balle afin de déterminer clairement ce qui a été introduit et ce qui a été modifié.

## Modèle

Renseignez les espaces réservés (ne laissez pas de crochets d’angle dans le message final) :

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## Exemple

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
