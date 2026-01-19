# ⚙️ Configuration du Système

Cette section présente les étapes essentielles de la configuration d’un système informatique,
depuis le démarrage matériel jusqu’à la sécurité et la sauvegarde des données.

---

## 🧩 Configuration BIOS / UEFI

### 🎯 Objectif
Le BIOS (Basic Input/Output System) ou l’UEFI (Unified Extensible Firmware Interface)
est le premier logiciel qui s’exécute au démarrage de l’ordinateur.
Il initialise les composants matériels (CPU, RAM, disque, clavier…)
et prépare le chargement du système d’exploitation.

### 🔑 Accès
L’accès au BIOS/UEFI se fait au démarrage de l’ordinateur
en appuyant sur une touche spécifique selon le fabricant :
- **F2**
- **F10**
- **F12**
- **Suppr (Delete)**

### ⚙️ Paramètres courants
- **Ordre de démarrage (Boot Order)** : choix du périphérique de démarrage (HDD, SSD, USB, DVD)
- **Activation / Désactivation du matériel** : USB, carte réseau, virtualisation
- **Gestion de l’alimentation** : économie d’énergie, veille
- **Paramètres de performance** : fréquence CPU, RAM, options avancées

---

## 💽 Partitionnement et Formatage

### 📦 Partitionnement de disque
Le partitionnement consiste à diviser un disque physique
en plusieurs parties logiques indépendantes.
Chaque partition peut contenir un système ou des données différentes.

### 🗂️ Types de tables de partition
- **MBR (Master Boot Record)**  
  Standard ancien, limité à **2 To** par partition et 4 partitions primaires.
- **GPT (GUID Partition Table)**  
  Standard moderne, supporte des disques très volumineux
  et un grand nombre de partitions. Recommandé avec UEFI.

### 🗃️ Systèmes de fichiers
Les systèmes de fichiers organisent le stockage des données sur les partitions.

- **Windows** : NTFS, FAT32, exFAT
- **Linux** : ext4, XFS, Btrfs
- **Multiplateforme** : exFAT (compatible Windows / Linux / macOS)

---

## 🌐 Configuration Réseau

### 🌍 Adressage IP
- **IP statique** :  
  Adresse réseau fixe configurée manuellement.
  Utilisée pour les serveurs et équipements critiques.
- **DHCP** :  
  Adresse attribuée automatiquement par un serveur DHCP.
  Simplifie la gestion du réseau pour les utilisateurs.

### 🔎 Configuration DNS
Les serveurs DNS traduisent les noms de domaine
(ex : google.com) en adresses IP compréhensibles par les machines.

### 🛠️ Outils de diagnostic réseau
- **ping** : vérifie la connectivité entre deux machines
- **traceroute / tracert** : affiche le chemin réseau vers une destination
- **ipconfig / ifconfig** : affiche la configuration réseau
- **nslookup** : teste la résolution DNS

---

## 🔐 Sécurité de Base

### 🧱 Pare-feu (Firewall)
Le pare-feu filtre le trafic réseau entrant et sortant
selon des règles définies pour protéger le système
contre les accès non autorisés.

### 🛡️ Antivirus / Antimalware
Logiciels de sécurité qui détectent, bloquent et suppriment
les virus, ransomwares, spywares et autres menaces.

### ⚠️ Paramètres de sécurité standards
- Mises à jour automatiques du système
- Politiques de mots de passe forts
- Verrouillage automatique de l’écran
- Gestion des comptes utilisateurs

---

## 💾 Solutions de Sauvegarde

### 📂 Types de sauvegarde
- **Sauvegarde complète** :  
  Copie intégrale de toutes les données sélectionnées.
- **Sauvegarde incrémentielle** :  
  Sauvegarde uniquement les modifications
  depuis la dernière sauvegarde.
- **Sauvegarde différentielle** :  
  Sauvegarde les modifications
  depuis la dernière sauvegarde complète.

### ☁️ Options de stockage
- Disques durs externes
- Stockage réseau (NAS)
- Services cloud (Google Drive, OneDrive, etc.)

### ⏰ Planification
La planification permet d’automatiser les sauvegardes
à intervalles réguliers afin d’éviter toute perte de données.
