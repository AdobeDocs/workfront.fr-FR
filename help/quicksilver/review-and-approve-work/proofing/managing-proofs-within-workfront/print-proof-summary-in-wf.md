---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Imprimer un résumé du BAT dans Adobe Workfront
description: Vous pouvez imprimer un résumé du BAT, l’enregistrer en tant que PDF ou l’exporter en tant que fichier XLS ou PDF optimisé pour Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

---

# Imprimer un résumé du BAT dans Adobe Workfront

Vous pouvez imprimer un résumé du BAT, l’enregistrer en tant que PDF ou l’exporter en tant que fichier XLS ou PDF optimisé pour Adobe Reader.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou version ultérieure</p> <p>ou</p> <p>Plan hérité : Sélectionner ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Travail ou plan</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Imprimer un résumé du BAT ou l’enregistrer en tant que fichier PDF

Vous pouvez imprimer un résumé du BAT directement à partir de la liste des documents.

>[!NOTE]
>
>Vous ne pouvez pas imprimer simultanément plusieurs résumés de BAT à partir de la liste de documents.

1. Dans la liste des documents qui contient le BAT, passez la souris sur la ligne contenant le document, puis cliquez sur **Résumé de l’impression**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Ou

   Lors de l’affichage du BAT dans la visionneuse de vérification, cliquez sur le bouton **Imprimer** icon ![](assets/print-icon-in-pv.png) dans la barre d’outils de gauche. (Si la barre d’outils de gauche n’est pas visible, cliquez sur l’icône Menu ![](assets/menu-icon-in-pv.png) dans le coin supérieur gauche de la visionneuse de vérification).

1. Utilisez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher</td> 
      <td> <p>Indiquez ce que vous souhaitez imprimer :</p> 
       <ul> 
        <li>Le <strong>Version actuelle</strong> ou <strong>Toutes les versions</strong> du BAT</li> 
        <li>Seule la variable <strong>Pages avec commentaires</strong> ou <strong>Toutes les pages</strong></li> 
        <li>Seule la variable <strong>Miniatures de page</strong> (un petit rendu de chaque page) ou <strong>Pages complètes</strong> (un rendu complet du BAT)<br></li> 
        <p>Remarque : Pour afficher les numéros d’épingles sur les balises dans la sortie imprimée, vous devez sélectionner Pages complètes, et non Miniatures de page. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trier les commentaires par</td> 
      <td> <p>(Disponible uniquement si vous avez sélectionné Miniatures de page ci-dessus) Indiquez l’ordre d’impression des commentaires du BAT :</p> 
       <ul> 
        <li><strong>Plus ancien</strong>: Du premier commentaire effectué à la dernière</li> 
        <li><strong>Dernière</strong>: Du dernier commentaire effectué au premier</li> 
        <li><strong>Page</strong>: Par page, de la première page à la dernière ou de la dernière page à la première</li> 
        <li><strong>Créateur</strong>: Par les noms des utilisateurs qui les ont ajoutés, de A-Z ou de Z-A</li> 
       </ul> <p>Ces options n’affectent pas la sortie que vous exportez en tant que fichier XLS ou PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtrage des commentaires par</td> 
      <td> <p>Vous pouvez utiliser n’importe quelle combinaison de ces options pour inclure uniquement certains commentaires dans la sortie que vous imprimez ou exportez en tant que fichier XLS ou PDF :</p> 
       <ul> 
        <li>Auteurs sélectionnés (par défaut)</li> 
        <li>Actions sélectionnées</li> 
        <li><strong>Non résolu</strong> status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flux de travail</td> 
      <td> <p>(Disponible uniquement si le BAT comporte un workflow automatisé) Vous pouvez cliquer sur <strong>Afficher le diagramme</strong> pour inclure un diagramme en sortie imprimée montrant les étapes du BAT et les décisions prises à chaque étape. Dans le diagramme qui s’affiche, les couleurs représentent les décisions prises sur une scène :</p> <p><strong>Vert</strong>: Approuvé</p> <p><strong>Bleu</strong>: En attente de décision</p> <p><strong>Rouge</strong>: Modifications de la décision requise</p> <p><strong>Gris</strong>: Pas encore commencé</p> <p><strong>Jaune</strong>: Approuvé avec modifications</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Imprimer**.
1. Dans le panneau de droite de la fenêtre qui s’affiche, si vous souhaitez imprimer la synthèse, cliquez sur le bouton **Destination** , puis cliquez sur **En savoir plus**. Cliquez sur l’imprimante à utiliser dans la liste qui s’affiche, puis cliquez sur **Imprimer**.

   Ou

   Si vous souhaitez enregistrer le résumé en tant que fichier de PDF, cliquez sur le bouton **Destination** , cliquez sur **Enregistrer en tant que PDF**, puis cliquez sur **Enregistrer**.

## Exportation d’un résumé de BAT au format XLS ou PDF

Vous pouvez exporter un résumé du BAT pour le contenu statique sous la forme d’un fichier XLS ou d’un fichier de PDF. Les exports de BAT ne comprennent que le contenu du BAT.

1. Dans la liste des documents qui contient le BAT, passez la souris sur la ligne contenant le document, puis cliquez sur **Résumé de l’impression**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Cliquez sur l’icône XLS ou l’icône de PDF près du coin supérieur droit de la page.

   ![](assets/xls-pdf-icons-350x136.png)

Lorsque le fichier exporté est prêt, vous recevez un e-mail à partir duquel vous pouvez télécharger le fichier.

Si vous avez exporté la synthèse en tant que fichier de PDF, les commentaires sur le BAT apparaissent dans le lecteur du PDF. Si un commentaire est associé à plusieurs balises, celui-ci apparaît plusieurs fois dans la liste des commentaires (une fois pour chaque balise).
