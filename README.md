# AdminScript DOC

# Documentation Script Gestion Active Directory

Le script de gestion d'Active Directory est composé d'un menu et de sous-menus ayant pour but de créer, modifier et/ou supprimer des unités d'organisation (OU), des groupes et des utilisateurs.

## Fonctionnalités principales

### Gestion des OU

- **Création** : `create-ou` demande le nom et l'emplacement (DN) de l'OU à créer.
- **Modification** : `modify-ou` permet de renommer une OU existante.
- **Suppression** : `remove-ou` supprime une OU en spécifiant son DN.

### Gestion des groupes

- **Création** : `create-group` demande le nom, la portée et l'emplacement du groupe.
- **Modification** : `modify-group` permet de renommer et/ou déplacer un groupe existant.
- **Suppression** : `remove-group` supprime un groupe après confirmation.

### Gestion des utilisateurs

- **Création** : `Create-User` crée un nouvel utilisateur avec nom, SAM, mot de passe et emplacement.
- **Modification** : `Modify-User` permet de modifier le nom et l'emplacement d'un utilisateur existant.
- **Suppression** : `Remove-User` supprime un compte utilisateur après confirmation.
- **Réinitialisation du mot de passe** : `Reset-UserPassword` permet de changer le mot de passe d'un utilisateur.
- **Activation/Désactivation** : `Toggle-UserAccount` active ou désactive un compte utilisateur.
- **Gestion des groupes** : `Modify-UserGroups` permet d'ajouter ou retirer un utilisateur d'un groupe.

## Navigation et sécurité

- Le script utilise un menu interactif avec des vérifications à chaque étape pour éviter les erreurs.
- **Attention** : toutes les actions sont irréversibles.

## Structure du script

Le script fonctionne par appels de fonctions dans l'ordre défini. Chaque fonction gère une opération spécifique sur les objets AD (OU, groupes, utilisateurs).

## Paramètres importants

- Pour les utilisateurs, le SAM (Security Account Manager) est un identifiant crucial utilisé dans plusieurs fonctions.
- Pour les OU et les groupes, le DN (Distinguished Name) est souvent requis pour les opérations.


