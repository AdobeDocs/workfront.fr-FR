---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules SFTP
description: Les modules  [!DNL Adobe Workfront Fusion SFTP]  vous permettent de surveiller les modifications de fichier dans un (sous-)dossier sélectionné, de charger de nouveaux fichiers dans le dossier souhaité, de modifier ou de supprimer des fichiers existants qui se trouvent déjà dans un dossier ou de modifier les autorisations de fichier.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1920'
ht-degree: 100%

---

# Modules SFTP

Les modules [!DNL Adobe Workfront Fusion]SFTP vous permettent de surveiller les modifications de fichier dans un (sous-)dossier sélectionné, de charger de nouveaux fichiers dans le dossier souhaité, de modifier ou de supprimer des fichiers existants qui se trouvent déjà dans un dossier ou de modifier les autorisations de fichier.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser SFTP avec [!DNL Workfront Fusion], il est nécessaire d’avoir un compte SFTP (comme l’hébergement web [!DNL GoDaddy]).

## Connecter SFTP à [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Pour connecter votre compte SFTP à [!DNL Workfront Fusion], vous devez saisir l’hôte cible et les informations d’identification SFTP (nom d’utilisateur ou d’utilisatrice et mot de passe ou nom d’utilisateur ou d’utilisatrice et clé) pour la boîte de dialogue [!UICONTROL Créer une connexion] du module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection name]</td> 
   <td> <p> Saisissez le nom de votre connexion SFTP.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>Saisissez le nom d’hôte du serveur SFTP que vous souhaitez connecter.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Saisissez le port du serveur SFTP. Par exemple, 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Auth type]</p> </td> 
   <td> <p>Sélectionnez le mode d’autorisation à utiliser pour la connexion au serveur SFTP.</p> 
    <ul> 
     <li><strong>[!UICONTROL User name and password]</strong> : saisissez vos informations d’identification.</li> 
     <li> <p><strong>[!UICONTROL User name and key]</strong> : saisissez votre nom d’utilisateur ou d’utilisatrice et votre clé privée/certificat privé.</p> <p>Chargez la clé privée pour utiliser l’autorisation côté client ou chargez votre certificat (fichier P12 ou PFX) si vous souhaitez utiliser TLS à l’aide de votre certificat auto-signé. Si vous utilisez l’autorisation de certificat côté client, vous pouvez saisir votre certificat d’autorité de certification ici.</p> <p>[!DNL Workfront Fusion] ne conserve ni ne stocke les données (fichiers, mots de passe) fournies ici. Le fichier et le mot de passe ne sont utilisés que pour extraire une clé privée/un certificat privé.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Après avoir saisi les informations de connexion, cliquez sur **[!UICONTROL Continuer]** pour établir une connexion.

## Modules [!UICONTROL SFTP] et leurs champs

Lorsque vous configurez les modules [!UICONTROL SFTP], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En outre, des champs [!UICONTROL SFTP] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheurs

#### [!UICONTROL Surveiller les fichiers dans un dossier]

Renvoie les fichiers avec des détails lorsqu’un fichier est créé ou modifié dans un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier que vous souhaitez surveiller. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Taille de la mémoire tampon [B]</td> 
   <td> <p> Saisissez la taille de la mémoire tampon en octets. Cette valeur définit la taille des morceaux transférés depuis le serveur. Certains serveurs peuvent causer des problèmes ou corrompre des fichiers lorsque la valeur est trop élevée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files]</td> 
   <td> <p> Définissez le nombre maximal de fichiers avec lesquels [!DNL Workfront Fusion] fonctionnera pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les sous-dossiers dans un dossier]

Renvoie des dossiers avec des détails lorsqu’un dossier est créé ou modifié dans un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier que vous souhaitez surveiller. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files]</td> 
   <td> <p> Définissez le nombre maximum de dossiers que [!DNL Workfront Fusion] renverra pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

#### [!UICONTROL Lister le contenu d’un dossier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Sélectionnez si vous souhaitez récupérer des fichiers, des dossiers ou les deux.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier qui contient les fichiers ou les dossiers à répertorier. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Saisissez ou mappez le terme de recherche. Par exemple, si vous souhaitez rechercher des fichiers portant l’extension .txt, saisissez <code>.txt</code>.Vous pouvez également saisir ou mapper le nom du fichier que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort By]</td> 
   <td> <p> Indiquez si vous souhaitez trier les résultats par nom de fichier, taille, date de dernier accès ou date de dernière modification.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort Order] </td> 
   <td> <p>Indiquez si le résultat doit être renvoyé par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continue the execution of the route even if the module returns no results]</p> </td> 
   <td>Activez cette option pour vous assurer que ce module n’arrête pas le scénario s’il ne renvoie aucun résultat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td> <p> Définissez le nombre maximum de résultats que [!DNL Workfront Fusion] renverra pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des fichiers]

Ce module répertorie les fichiers d’un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buffer Size [B]]</td> 
   <td> <p> Saisissez la taille de la mémoire tampon en octets. Cette valeur définit la taille des morceaux transférés depuis le serveur. Certains serveurs peuvent causer des problèmes ou corrompre des fichiers lorsque la valeur est trop élevée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier qui contient les fichiers ou les dossiers à répertorier. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Saisissez ou mappez le terme de recherche. Par exemple, si vous souhaitez rechercher des fichiers portant l’extension .txt, saisissez <code>.txt</code>.Vous pouvez également saisir ou mapper le nom du fichier que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort By]</td> 
   <td> <p> Indiquez si vous souhaitez trier les résultats en fonction du nom du fichier, de sa taille, de la date du dernier accès ou de la date de la dernière modification.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort Order]</td> 
   <td> <p> Indiquez si le résultat doit être renvoyé par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continue the execution of the route even if the module returns no results]</p> </td> 
   <td>Activez cette option pour vous assurer que ce module n’arrête pas le scénario s’il ne renvoie aucun résultat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td> <p> Définissez le nombre maximum de fichiers que [!DNL Workfront Fusion] renvoie au cours d’un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un fichier]

Ce module permet de récupérer les détails d’un fichier, y compris ses données.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buffer Size [B]]</td> 
   <td> <p> Saisissez la taille de la mémoire tampon en octets. Cette valeur définit la taille des morceaux transférés depuis le serveur. Certains serveurs peuvent causer des problèmes ou corrompre des fichiers lorsque la valeur est trop élevée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path] </td> 
   <td> <p>Saisissez le chemin d’accès au fichier. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Charger un fichier]

Ce module permet de charger un fichier vers le serveur SFTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Spécifiez un dossier existant comme emplacement de stockage du fichier. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source File]</td> 
   <td> <p> Mappez le fichier source d’un module précédent, tel que [!UICONTROL Dropbox] &gt; [!UICONTROL Get File]. Vous pouvez également saisir ou mapper le nom et les données du fichier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Définissez les autorisations souhaitées pour le fichier ou le dossier. Utilisez les paramètres chmod. Par exemple, <code>777 </code> ou <code>-rwxrwxrwx</code>.</p> <p>Pour plus de détails sur chmod, voir la <a href="https://ss64.com/bash/chmod.html">documentation chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Renommer un fichier]

Renomme un fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez renommer. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New file name]</td> 
   <td> <p> Saisissez le nouveau nom du fichier, y compris son extension.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez déplacer. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New Folder]</td> 
   <td> <p> Saisissez le chemin d’accès au nouvel emplacement du fichier. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un fichier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez supprimer. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour les autorisations d’un fichier]

Permet de modifier les autorisations du fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez déplacer. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Définissez les autorisations de fichier souhaitées. Utilisez les paramètres chmod. Par exemple, saisissez <code>777 </code> ou <code>-rwxrwxrwx</code>.</p> <p>Doit correspondre au modèle <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Pour plus de détails sur chmod, veuillez vous référer à la <a href="https://ss64.com/bash/chmod.html">documentation chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un dossier]

Crée un nouveau dossier à l’emplacement spécifié.

>[!NOTE]
>
>Si le dossier existe déjà, le module renvoie une erreur. Pour poursuivre le flux sans interruption, associez un itinéraire de gestionnaire d’erreurs au module afin de détecter l’erreur et utilisez la directive [!UICONTROL Resume] pour poursuivre le flux. Pour plus d’informations sur l’association d’un itinéraire de gestionnaire d’erreurs, voir [Gérer les erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Pour plus d’informations sur l’itinéraire de gestionnaire d’erreurs, voir [Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Spécifiez un dossier existant comme emplacement de stockage pour le nouveau dossier. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name]</td> 
   <td> <p> Saisissez le nom du dossier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Définissez les autorisations souhaitées pour le dossier. Utilisez les paramètres chmod. Par exemple, <code>777 </code> ou <code>-rwxrwxrwx</code>.</p> <p>Doit correspondre au modèle <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Pour plus de détails sur chmod, voir la <a href="https://ss64.com/bash/chmod.html">page du manuel chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un dossier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour savoir comment connecter votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Indiquez le chemin d’accès au dossier à supprimer. Vous pouvez spécifier un chemin d’accès absolu tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de la personne connectée, tel que <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
