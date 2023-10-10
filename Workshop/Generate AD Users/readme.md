# Exercice

A partir d'une API renvoyant des utilisateurs aléatoire, créer des utilisateurs AD.

## API

URL: `https://randomuser.me/api/?results=10&nat=FR`

## OU

Les utilisateurs devront être crées dans une sous OU à votre nom de l'OU _OU=Services,DC=contoso,DC=com_  qui devra être crée au besoin.

## Propriétés ADUser

| Property          | Format                           |
| ----------------- | -------------------------------- |
| DisplayName       | "Prénom Nom"                     |
| Name              | "Prénom Nom"                     |
| SamAccountName    | "pnom" (attention aux accents)   |
| Surname           | Nom                              |
| GivenName         | Prénom                           |
| UserPrincipalName | "SamAccountName@_DomainDNSRoot_" |
| Path              | Votre OU                         |
| AccountPassword   | Password **aléatoire**             |
| Enabled           | **$true**                         |

