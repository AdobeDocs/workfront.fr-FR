---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Imprimer un résumé des épreuves dans Adobe Workfront
description: Vous pouvez imprimer un résumé d’épreuve, l’enregistrer au format PDF ou l’exporter dans un format XLS ou PDF optimisé pour Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 93%

---

# Imprimer un résumé des épreuves dans Adobe Workfront

Vous pouvez imprimer un résumé d’épreuve, l’enregistrer au format PDF ou l’exporter dans un format XLS ou PDF optimisé pour Adobe Reader.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan actuel : Pro ou version supérieure</p> <p>ou</p> <p>Formule héritée : Select ou Premium</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice Workfront ou Workfront Proof.

+++

## Imprimer un résumé d’épreuve ou l’enregistrer au format PDF

Vous pouvez imprimer un résumé d’épreuve directement à partir de la liste des documents.

>[!NOTE]
>
>* Les résumés de plus de 1 Go ne sont pas pris en charge.
>* Plusieurs résumés d’épreuves ne peuvent pas être imprimés simultanément à partir de la liste des documents.

1. Dans la liste des documents contenant l’épreuve, pointez sur la ligne contenant le document, puis cliquez sur **Imprimer le résumé**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Ou

   Lors de l’affichage du BAT dans la visionneuse de BAT, cliquez sur l’icône **Imprimer** icône ![Imprimer](assets/print-icon-in-pv.png) dans la barre d’outils de gauche. (Si la barre d&#39;outils de gauche n&#39;est pas visible, cliquez sur l&#39;icône Menu ![icône Menu](assets/menu-icon-in-pv.png) dans le coin supérieur gauche de la visionneuse de relecture.)

1. Utilisez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher</td> 
      <td> <p>Indiquez ce que vous souhaitez imprimer :</p> 
       <ul> 
        <li>La <strong>Version actuelle</strong> ou <strong>Toutes les versions</strong> de l’épreuve</li> 
        <li>Seules les <strong>Pages avec commentaires</strong> ou <strong>Toutes les pages</strong></li> 
        <li>Seules les <strong>Miniatures des pages</strong> (un petit rendu de chaque page) ou les <strong>Pages complètes</strong> (un rendu complet de l’épreuve)<br></li> 
        <p>Note : pour que les numéros d’épingle des marques apparaissent dans votre document imprimé, vous devez sélectionner les pages complètes, et non les miniatures. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trier les commentaires par</td> 
      <td> <p>(Disponible uniquement si vous avez sélectionné les miniatures de page ci-dessus) Indiquez l’ordre dans lequel vous souhaitez que les commentaires de l’épreuve s’impriment :</p> 
       <ul> 
        <li><strong>Le plus ancien</strong> : du premier commentaire au dernier</li> 
        <li><strong>Le plus récent</strong> : du dernier commentaire au premier</li> 
        <li><strong>Page</strong> : par page, de la première page à la dernière ou de la dernière page à la première</li> 
        <li><strong>Créateur ou créatrice</strong> : par les noms des utilisateurs et des utilisatrices qui les ont ajoutés, de A-Z ou de Z-A</li> 
       </ul> <p>Ces options n’affectent pas les résultats exportés sous forme de fichiers XLS ou PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtrer les commentaires par</td> 
      <td> <p>Vous pouvez utiliser une combinaison de ces options pour n’inclure que certains commentaires dans le résultat que vous imprimez ou que vous exportez sous la forme d’un fichier XLS ou PDF :</p> 
       <ul> 
        <li>Personnes chargées de la création sélectionnées (par défaut)</li> 
        <li>Actions sélectionnées</li> 
        <li>Statut <strong>non résolu</strong></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workflow</td> 
      <td> <p>(Disponible uniquement si l’épreuve a un workflow automatisé) Vous pouvez cliquer sur <strong>Afficher le diagramme</strong> pour inclure un diagramme dans la sortie imprimée montrant les étapes de l’épreuve et les décisions prises à chaque étape. Dans le diagramme qui apparaît, les couleurs représentent les décisions prises à une étape :</p> <p><strong>Vert</strong> : approuvé</p> <p><strong>Bleu</strong>: en attente de décision</p> <p><strong>Rouge</strong> : décision de modification requise</p> <p><strong>Gris</strong> : pas encore commencé</p> <p><strong>Jaune</strong> : approuvé avec des modifications</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Imprimer**.
1. Dans le panneau de droite de la fenêtre qui s’affiche, si vous souhaitez imprimer le résumé, cliquez sur le menu **Destination**, puis sur **Voir plus**. Cliquez sur l’imprimante que vous souhaitez utiliser dans la liste qui s’affiche, puis cliquez sur **Imprimer**.

   Ou

   Si vous souhaitez enregistrer le résumé sous forme de fichier PDF, cliquez sur le menu **Destination**, cliquez sur **Enregistrer en tant que fichier PDF**, puis cliquez sur **Enregistrer**.

## Exporter un résumé d’épreuve au format XLS ou PDF

Vous pouvez exporter un résumé d’épreuve pour le contenu statique sous la forme d’un fichier XLS ou d’un fichier PDF. Les exports d’épreuves ne comprennent que le contenu de l’épreuve.

1. Dans la liste des documents contenant l’épreuve, pointez sur la ligne contenant le document, puis cliquez sur **Imprimer le résumé**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Cliquez sur l’icône XLS ou PDF dans le coin supérieur droit de la page.

   ![Icône XLS PDF](assets/xls-pdf-icons-350x136.png)

Lorsque le fichier exporté est prêt, vous recevez un e-mail à partir duquel vous pouvez le télécharger.

Si vous avez exporté le résumé sous forme d’un fichier PDF, les commentaires sur l’épreuve apparaissent dans le lecteur PDF. Si un commentaire est associé à plusieurs annotations, il apparaîtra plusieurs fois dans la liste des commentaires (une fois pour chaque annotation).
