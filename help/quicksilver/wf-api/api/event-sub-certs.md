---
content-type: api
navigation-topic: api-navigation-topic
title: Certificats d’abonnement d’événement
description: Certificats d’abonnement d’événement
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Configuration du TLS client pour l’abonnement à un événement

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

Le TLS client vous permet de vérifier que le message d’abonnement à l’événement que vous recevez provient bien d’Adobe Workfront. Pour activer cette fonctionnalité, votre serveur doit être configuré pour demander et valider le certificat x509 de Workfront.


## Vérification du certificat client Workfront

Cette procédure suppose que votre serveur est configuré pour accepter les connexions TLS. Workfront ne prend pas en charge les certificats auto-signés.

En général, voici les étapes nécessaires pour activer l’authentification du client pour votre serveur :

1. Téléchargez la version PEM du certificat d’autorité de certification racine globale DigiCert.
1. Activez la vérification du certificat client.

   Spécifiez le certificat d’autorité de certification de l’étape 1 comme approuvé.

1. Définissez la profondeur de vérification sur 2 puisque notre certificat est en fait signé par l’autorité de certification du serveur sécurisé DigiCert SHA2 qui est une autorité de certification intermédiaire sous l’autorité de certification racine globale DigiCert.
1. Vérifiez que le certificat client provient bien de Workfront en examinant son nom de domaine d’objet.

## Exemples de configuration de serveur

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

Pour plus d’informations, voir [Documentation NGiNX pour ngx_http_ssl_module](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

Pour plus d’informations, voir

* [Authentification du client et contrôle d’accès](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Module Apache mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Mappage du certificat à l’environnement

| Environnement WF | Nom commun au certificat | Certificate Subject (DN) |
| -- | -- | -- |
| Production | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc/CN=*.prod.eventsubscriptions.workfront.com |
| Aperçu | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc/CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc/CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc/CN=*.sandbox.eventsubscriptions.workfront.com |

## Téléchargement de certificats

Cliquez sur les liens suivants pour télécharger les certificats client.

* [Certificat client - Environnement de production](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [Client certificate - Preview environment](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [Certificat client - Environnement Sandbox](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>Vous pouvez utiliser le même certificat client pour les deux environnements Sandbox.
