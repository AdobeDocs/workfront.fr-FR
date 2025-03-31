---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Créer un compte de lecteur pour Snowflake
description: Pour accéder aux données de Data Connect, vous devez d’abord créer un compte de lecteur Snowflake.
author: Courtney
feature: Reports and Dashboards
hide: true
hidefromtoc: true
source-git-commit: a42c13804b0463af27bac6f9166bc6e3c41d3fda
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 8%

---


# Test

## Niveaux d&#39;accès

<table>
  <thead>
    <tr>
        <th>Nom de l’entité Workfront</th>
        <th>Références d’interface</th>
        <th>Référence d’API | Libellé</th>
        <th>Vues du lac de données</th>
    </tr>
  </thead>
 <tr>
        <td>Niveau d’accès</td>
         <td>Niveau d’accès</td>
        <td>ACSLVL | Niveau d'accès</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>Champ Relations</strong> <br>
         ACCESSLEVELID (self) : Self<br>
         APPGLOBALID : n’est pas une relation ; utilisé à des fins d’application interne<br>
         LASTUPDATEDBYID : USER_CURRENT | USERID <br>
         LEGACYACCESSLEVELID : n’est pas une relation ; utilisé à des fins d’application interne<br>
         OBJID : ID de l’objet identifié dans le champ OBJCODE <br>
         SYSID : non une relation ; utilisé à des fins d’application interne</td>
    </tr>
</table>

## Niveaux d&#39;accès

<table>
  <thead>
    <tr>
        <th>Nom de l’entité Workfront</th>
        <th>Références d’interface</th>
        <th>Référence d’API | Libellé</th>
        <th>Vues du lac de données</th>
    </tr>
  </thead>
 <tr>
        <td>Niveau d’accès</td>
         <td>Niveau d’accès</td>
        <td>ACSLVL | Niveau d'accès</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>Champ Relations</strong> <br>
         <ul>
            <li>ACCESSLEVELID (self) : Self</li>
            <li>APPGLOBALID : non une relation ; utilisé à des fins d’application interne</li>
            <li>LASTUPDATEDBYID : USER_CURRENT | USERID</li>
            <li>LEGACYACCESSLEVELID : n’est pas une relation ; utilisé à des fins d’application interne</li>
            <li>OBJID : ID de l’objet identifié dans le champ OBJCODE</li>
            <li>SYSID : non une relation ; utilisé à des fins d’application interne</li>
        </ul>
    </tr>
</table>