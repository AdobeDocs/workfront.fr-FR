---
content-type: api
navigation-topic: api-navigation-topic
title: Certificats d’inscription à des événements
description: Certificats d’inscription à des événements
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 0921cc0e45a0a845404df90fc8789efc764f5790
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 88%

---

# Configurer le TLS client pour l’abonnement à un événement

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

Le TLS client vous permet de vérifier que le message d’abonnement à un événement que vous recevez provient bien d’Adobe Workfront. Pour activer cette fonctionnalité, votre serveur doit être configuré pour demander et valider le certificat x509 de Workfront.


>[!NOTE]
>
>Les abonnements aux événements utilisent TLS version 1.3 si le serveur auquel l’abonnement aux événements envoie des événements prend en charge la version 1.3. Si le serveur de connexion ne prend pas en charge la version 1.3, l’abonnement aux événements utilise la version 1.2 de TLS.



## Vérifier le certificat client de Workfront

Avant d’exécuter cette procédure, assurez-vous que votre serveur est configuré pour accepter les connexions TLS. Workfront ne prend pas en charge les certificats auto-signés.

En général, les étapes nécessaires pour activer l’authentification du client pour votre serveur sont les suivantes :

1. Téléchargez la version PEM du certificat d’autorité de certification de racine globale DigiCert.
1. Activez la vérification du certificat client.

   Indiquez le certificat d’autorité de certification de l’étape 1 comme approuvé.

1. Définissez la profondeur de vérification sur 2, puisque notre certificat est en fait signé par l’autorité de certification du serveur sécurisé DigiCert SHA2, qui est une autorité de certification intermédiaire sous l’autorité de certification racine globale DigiCert.
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

Pour plus d’informations, voir [Documentation NGiNX pour ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html).

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

Pour plus d’informations, consultez les ressources suivantes :

* [Authentification du client et contrôle d’accès](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Module Apache mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Mappage du certificat à l’environnement

| Environnement WF | Nom courant du certificat | Objet du certificat (DN) |
| -- | -- | -- |
| Production | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Aperçu | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Télécharger des certificats

Cliquez sur les liens suivants pour télécharger des certificats client.

* [Certificat client - Environnement de production](assets/prod-ES-client-cert-oct25.crt)
* [Certificat client - Environnement de prévisualisation](assets/preview-ES-client-cert-oct25.crt)
* [Certificat client - Environnement de sandbox](assets/sandbox-ES-client-cert-oct25.crt)

>[!NOTE]
>
>Vous pouvez utiliser le même certificat client pour les deux environnements de sandbox.
