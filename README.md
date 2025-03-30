
![image](https://github.com/user-attachments/assets/5a300f0f-4b45-41de-8357-fb5b87a1dc9b)


---

# Documentation d'Installation de Wazuh SIEM sur Ubuntu 22.04.

## Introduction

Wazuh est une solution open source de SIEM (Security Information and Event Management) puissante et flexible, conçue pour la détection de menaces, la réponse aux incidents et la gestion de la conformité.

---

## 1. Préparation de l'environnement

### a. Installation d'Ubuntu 22.04. LTS

- Téléchargez la dernière version d'Ubuntu 22.04. 
- Installez Ubuntu sur le serveur physique ou virtuel.Dans notre cas sur un environnement Proxmox

### b. Mise à jour des dépôts APT

Avant toute installation, il est essentiel de mettre à jour les sources de paquets pour obtenir les dernières versions des logiciels disponibles.  
On Ouvre un terminal et exécutez :

```bash
sudo apt update
```


---

## 2. Installation rapide avec l'assistant d'installation Wazuh

Pour simplifier l'installation, Wazuh propose un script d'assistant qui automatise la plupart des étapes :

a. **Téléchargement et exécution du script**  
   

   ```bash
   curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh && sudo bash ./wazuh-install.sh -a
   ```

b. **Accès à l'interface**  
   Une fois le script terminé, des identifiants vous seront affichés dans le terminal. Copiez ces identifiants.  
   Ensuite, on ouvre le navigateur et on se rend sur l'adresse suivante :

   ```
   https://ip_du_serveur>
   ```

   Puis on se connecte en utilisant les identifiants fournis pour accéder au tableau de bord Wazuh.
