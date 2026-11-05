---
description: Règles de formatage et de validation pour les notes de mise à jour d’Adobe Workfront (présentation, zone produit, planification et pages d’aspect).
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# Formateur de notes de mise à jour

Ces fichiers sont des **notes de mise à jour** et non des articles pratiques. N’appliquez **** le
normes générales de qualité d&#39;écriture ici. Avant de procéder à la modification, lisez la source complète de
la vérité, qui inclut les modèles et le calendrier des versions :

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## Règle critique — déterminez d&#39;abord le trimestre doc

> [!IMPORTANT]
> N’affectez jamais une fonctionnalité à un document-trimestre à l’aide des mathématiques de trimestre calendaire sur son
> Date d’aperçu ou de production. Doc-quarter est basé sur la version **mensuelle)**
> la fonctionnalité est livrée, par regroupement interne calendrier de publication de Workfront, ce qui
> est décalé par rapport au trimestre calendaire. Par exemple, une fonctionnalité avec une production
> La date du 13 août 2026 appartient au doc-trimestre `26-q4`, et non au `26-q3`. Toujours
> vérifiez le tableau Calendrier des versions 2026 dans le fichier de référence avant
> la création ou la modification de n’importe quel fichier. Si une date de production ne figure pas dans ce tableau,
> demandez un calendrier à jour plutôt que de faire des suppositions.

## Règles structurelles clés

- **FrontMATTER** : `feature` doit être exactement `Product Announcements` ;
  `recommendations` doit être exactement `noDisplay, noCatalog`. Ne jamais inventer un
  `exl-id` — ne l&#39;inclure que s&#39;il en existe déjà un.
- **Fonctionnalités les plus récentes en premier** : la note de mise à jour la plus récente est le premier H2 après
l’introduction (pages de la zone produit) et la ligne supérieure de chaque tableau des fonctionnalités (aperçu)
pages).
- **Lien d’aperçu** : les pages produit doivent renvoyer vers **de leur propre trimestre**
fichier d&#39;aperçu — un bug courant est lié au trimestre précédent.
- **Légende de date** : chaque fonction H2 est suivie d&#39;un bloc de `>[!NOTE]` avec
Aperçu / Production Version rapide / Production pour toutes les dates, correspondant au
vue d’ensemble de la ligne du tableau. Formater les dates en `Month Day, Year` ; utiliser `TBD` si inconnu.
- **Noms écrits des trimestres** en H1s : « Premier trimestre », « Deuxième trimestre », « Troisième trimestre »
Trimestre », « Quatrième Trimestre ».

## Mises à jour complémentaires requises lors de l’ajout de pages

- **Nouvelle page (quelconque)** : ajoutez-la à `help/quicksilver/TOC.md` dans la même modification
(présentation en premier, pages par domaine de produits par ordre alphabétique, autres améliorations en dernier).
- **Page de présentation du nouveau trimestre** : mettez également à jour `help/quicksilver/home.md` —
actualisez le lien de l’onglet « Dernière version » et le lien de l’activité de planification, puis ajoutez :
le nouveau trimestre de l’onglet versions de l’année en cours.

Consultez les fichiers SKILL.md et reference.md ci-dessus pour obtenir les modèles complets,
conventions de dénomination des fichiers, formats de lien et calendrier de publication complet.
