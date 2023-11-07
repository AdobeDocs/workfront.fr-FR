---
content-type: api
navigation-topic: api-navigation-topic
title: Caractères échappés dans les réponses de l’API
description: Caractères échappés dans les réponses de l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# Caractères échappés dans les réponses de l’API

La syntaxe de certaines réponses de l’API peut contenir le caractère d’échappement, `\` (barre oblique inverse). Un caractère d’échappement indique que le caractère ou la chaîne de caractères qui suit immédiatement le caractère avec échappement ont une valeur spéciale. Par exemple : `\t` indique à l’appareil de lecture que `t` doit être interprété comme `tab` et non comme la lettre &quot;t&quot;. Une chaîne d’un ou plusieurs caractères suivant la barre oblique inverse est appelée séquence d’échappement.

Les séquences avec échappement hexadécimal nécessitent l’utilisation de chiffres hexadécimaux valides. Le tableau suivant répertorie les séquences d’échappement qui sont codées dans les réponses de l’API Adobe Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Séquence d’échappement</strong> </th> 
   <th><strong>Caractère Unicode</strong> </th> 
   <th><strong>Représente</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>Où, <em>x</em> est le code hexadécimal des nombres 0 à 7</p> </td> 
   <td>0-7</td> 
   <td>Caractères Unicode représentés par les points de code 0 à 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Revenir en arrière</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Onglet</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>Nouvelle ligne</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Onglet vertical</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Flux de formulaire</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Retour chariot</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Où, xx est le code hexadécimal des nombres 14 à 31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>Caractères Unicode représentés par les points de code 14 à 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (barre oblique)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (Inférieur à)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (barre oblique inverse)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>Où, <em>xxxx</em> est le code hexadécimal de tout nombre supérieur à 127.</p> </td> 
   <td>128+</td> 
   <td>Caractères Unicode pour tout point de code supérieur à 127</td> 
  </tr> 
 </tbody> 
</table>
