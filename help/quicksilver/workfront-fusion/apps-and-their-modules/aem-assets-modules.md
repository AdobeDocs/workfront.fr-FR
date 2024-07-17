---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Experience Manager Assets
description: Avec le connecteur  [!DNL Adobe Experience Manager Assets] pour le compte  [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] , créez, téléchargez et mettez à jour des ressources, et copiez ou déplacez des dossiers et des ressources.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1543'
ht-degree: 25%

---

# Modules [!DNL Adobe Experience Manager Assets]

Avec le connecteur [!DNL Adobe Experience Manager Assets] pour [!DNL Adobe Workfront Fusion], vous pouvez démarrer un scénario basé sur les événements de votre compte [!DNL Adobe Experience Manager Assets], créer, charger et mettre à jour des ressources, et copier ou déplacer des dossiers et des ressources.

Pour une présentation du connecteur Adobe Experience Manager Assets, voir :

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

* Vous devez disposer d’un compte [!DNL Adobe Experience Manager Assets] pour utiliser ces modules.
* Vous devez configurer le flux [!UICONTROL Serveur à serveur] dans [!DNL Adobe Developer console].

  Pour plus d&#39;informations sur la configuration du flux [!UICONTROL serveur à serveur] dans [!DNL Adobe Developer console], voir [ Génération de jetons d&#39;accès pour les API côté serveur](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connecter [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Pour créer une connexion pour vos modules [!DNL Adobe Experience Manager Assets] :

1. Cliquez sur [!UICONTROL Ajouter] en regard de la zone [!UICONTROL Connexion].

2. Sélectionnez le type de connexion que vous créez :

   * **[!DNL AEM Assets as a Cloud Service]**

     Cette configuration nécessite des informations de la [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     Cette configuration nécessite un nom d’utilisateur et un mot de passe.

3. Renseignez les champs correspondant au type de connexion que vous créez.

   Pour [!DNL AEM Assets as a Cloud Service], voir [Configuration de la connexion pour [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Pour [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services]), voir [ Configuration de la connexion pour [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.


### Configuration de la connexion pour [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>Les informations de ces champs sont générées dans le cadre de la configuration du flux [!UICONTROL Serveur à serveur] sur [!DNL Adobe Developer Console]. Vous pouvez trouver ces valeurs dans le fichier JSON des informations d’identification du service généré dans le cadre de cette configuration.
>
>Pour obtenir des instructions sur la configuration du flux [!UICONTROL serveur à serveur] sur [!UICONTROL Adobe Developer Console], voir [Génération de jetons d’accès pour les API côté serveur](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Connection name]</td>
                  <td>
                      <p>Saisissez le nom de cette connexion.</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL URL de l’instance sans barre oblique]</td>
                  <td>Saisissez l’URL de votre instance [!DNL Adobe Experience Manager]. N’incluez pas de barre oblique <code>/</code> à la fin de l’URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client ID]</td>
                  <td>Saisissez l’identifiant du client généré dans la configuration [!UICONTROL Server-to-server] .</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>Saisissez le secret client généré dans la configuration [!UICONTROL Server-to-server] .</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID du compte technique]</td>
                  <td>Saisissez l'identifiant du compte technique. Il s’agit du champ "[!UICONTROL id]" dans le fichier JSON des informations d’identification du client.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID d’organisation]</td>
                  <td class="">Saisissez l’ID de votre organisation. Il s’agit du champ "[!UICONTROL org]" dans le fichier JSON des informations d’identification du client.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Portées des métadonnées]</td>
                  <td>Saisissez les Métadonnées générées dans la configuration de [!UICONTROL Server-to-server] .</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Clé privée]</td>
                  <td>Saisissez la clé privée générée lors de la configuration de [!UICONTROL Server-to-server]. Pour extraire la clé privée, cliquez sur [!UICONTROL Extract], puis saisissez le fichier à extraire et le mot de passe du fichier.</td>
              </tr>
          </tbody>
      </table>


### Configuration de la connexion pour [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Connection name]</td>
                <td>
                    <p>Saisissez le nom de cette connexion.</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL de l’instance sans barre oblique]</td>
                <td>Saisissez l’URL de votre instance [!DNL Adobe Experience Manager]. N’incluez pas de barre oblique <code>/</code> à la fin de l’URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>Saisissez le nom d’utilisateur du compte [!DNL AEM Assets] utilisé par cette connexion.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>Saisissez le mot de passe du compte [!DNL AEM Assets] utilisé par cette connexion.</td>
            </tr>
        </tbody>
    </table>


## Modules [!DNL Adobe Experience Manager Assets] et leurs champs

Lorsque vous configurez des modules [!DNL Adobe Experience Manager Essentials], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Adobe Experience Manager Essentials] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Copier un dossier ou une ressource]

Ce module d’action copie un dossier ou une ressource vers un autre emplacement de votre compte Adobe Experience Manager Assets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Indiquez si vous souhaitez copier un dossier ou une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dossier] / [!UICONTROL Sélection de ressources]</td> 
   <td>Sélectionnez ou mappez le dossier ou la ressource à copier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chemin de destination]</td> 
   <td>Sélectionnez ou mappez le chemin d’accès à l’emplacement du nouveau dossier ou ressource.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du dossier copié] / [!UICONTROL ressource]</td> 
   <td>Saisissez le nom du nouveau dossier ou de la nouvelle ressource. Le nom du dossier qui s’affiche dans [!DNL Adobe Experience Manager Assets] est identique au nom d’origine. Le nom saisi ici apparaît dans l’URL du nouveau dossier ou de la nouvelle ressource.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copier les enfants]</td> 
   <td>Activez cette option pour copier tous les sous-dossiers ou ressources qu’il contient.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Remplacer]</td> 
   <td>Activez cette option pour remplacer un dossier ou une ressource de l’emplacement de destination qui porte le même nom que le dossier ou la ressource en cours de copie.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un dossier ou un commentaire de ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object type]</td> 
   <td> <p>Indiquez si vous souhaitez créer un dossier ou un commentaire sur une ressource.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Renseignez les champs suivants :</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Saisissez le nom du dossier. Ce nom apparaît dans le chemin d’accès au fichier. Il ne doit donc pas contenir d’espaces ni d’autres caractères. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>Saisissez le titre du dossier, qui peut s’afficher à la place du nom.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Commentaires sur la ressource]</p> <p>Renseignez les champs suivants :</p> 
      <ul> 
       <li> <p>[!UICONTROL Sélection de ressources]</p> <p>Sélectionnez ou mappez l’identifiant de la ressource à laquelle vous souhaitez ajouter un commentaire.</p> </li> 
       <li> <p>[!UICONTROL Comment]</p> <p>Saisissez le texte du commentaire.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un dossier, une ressource ou un rendu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Indiquez si vous souhaitez supprimer un dossier, une ressource ou un rendu.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Sélectionnez le dossier à supprimer en sélectionnant les dossiers dans son chemin.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Sélectionnez la ressource en sélectionnant les dossiers dans son chemin, puis la ressource à supprimer.</p> </li> 
     <li> <p>[!UICONTROL Rendu]</p> <p>Sélectionnez le rendu en sélectionnant les dossiers dans son chemin.</p> <p>Saisissez ou mappez le nom du rendu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtenir une liste de dossiers]

Ce module d’action récupère une représentation d’un dossier existant et de ses entités enfants (dossiers ou ressources).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Sélectionnez ou mappez le dossier que vous souhaitez récupérer. Pour ajouter des sous-dossiers au chemin d’accès, cliquez sur l’icône plus et sélectionnez le sous-dossier.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effectuer un appel d’API personnalisé]

Ce module d’action effectue un appel API personnalisé à l’API [!DNL Adobe Experience Manager Assets].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à l’URL de base [!DNL Adobe Experience Manager].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Saisissez la chaîne de requête de requête de requête. Pour chaque paire clé/valeur, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez la [!UICONTROL Clé] et la [!UICONTROL Valeur].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Déplacer un dossier ou une ressource]

Ce module d’action déplace la ressource ou le dossier à l’emplacement indiqué vers un nouvel emplacement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Indiquez si vous souhaitez déplacer un dossier ou une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset]</td> 
   <td>Sélectionnez ou mappez le dossier ou la ressource que vous souhaitez déplacer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chemin de destination]</td> 
   <td>Sélectionnez ou mappez le chemin d’accès à l’emplacement vers lequel vous souhaitez déplacer le dossier ou la ressource.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du dossier déplacé] / [!UICONTROL ressource]</td> 
   <td>Saisissez un nouveau nom pour le dossier ou la ressource déplacé. Le nom du dossier qui s’affiche dans [!DNL Adobe Experience Manager Assets] est identique au nom d’origine. Le nom saisi ici apparaît dans l’URL du dossier ou de la ressource déplacé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Remplacer]</td> 
   <td>Activez cette option pour remplacer un dossier ou une ressource de l’emplacement de destination qui porte le même nom que le dossier ou la ressource en cours de copie.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un enregistrement existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Indiquez si vous souhaitez supprimer des métadonnées de ressource ou un rendu de ressource.</p> 
    <ul> 
     <li> <p>[!UICONTROL Métadonnées de ressource]</p> 
      <ul> 
       <li> <p>Sélectionnez la ressource pour laquelle vous souhaitez mettre à jour les métadonnées.</p> </li> 
       <li> <p>Saisissez le nouveau titre de la ressource.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Rendu de ressource]</p> 
      <ul> 
       <li> <p>Sélectionnez la ressource pour laquelle vous souhaitez mettre à jour le rendu.</p> </li> 
       <li> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Télécharger une ressource]

Ce module d’action télécharge une ressource vers votre compte [!DNL Adobe Experience Manager Assets].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Adobe Experience Manager Assets] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination]</td> 
   <td> <p>Sélectionnez le dossier dans lequel vous souhaitez charger une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Saisissez ou mappez le nom et les données du fichier source.</td> 
  </tr> 
 </tbody> 
</table>
