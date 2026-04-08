---------------------------
##Projet
---------------------------
Notre projet porte sur le durcissement d'une vm Debian sans intervention manuel.

--------------------------
## Objectifs du playbook
---------------------------
- Mise à jour complète du système
- Désactivation de la connexion SSH root
- Désactivation de l'authentification SSH par mot de passe
- Configuration du pare-feu UFW avec règles minimales
- Installation et configuration de Fail2Ban et Tailscale
- Activation des mises à jour automatiques de sécurité
- Audit final avec Lynis et OpenSCAP

--------------------------
## Exécution du playbook
--------------------------
Depuis votre machine (Windows + WSL2 ou Linux) :

ansible-playbook -i inventory playbook.yml --ask-become-pass
