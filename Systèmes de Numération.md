# 🔢 Systèmes de Numération en Informatique

<img width="2056" height="1040" alt="Number_System" src="https://github.com/user-attachments/assets/b220a987-d7c3-4f70-a701-9aacf5752188" />

Les systèmes de numération sont des méthodes utilisées pour représenter
les nombres. En informatique, ils sont essentiels car les ordinateurs
ne comprennent que les signaux électriques (0 et 1).

---

## 🧠 Pourquoi les systèmes de numération sont importants ?

- L’ordinateur fonctionne uniquement en **binaire**
- Les réseaux, la sécurité et les systèmes utilisent
  différentes bases pour simplifier la lecture et la gestion
- Comprendre ces systèmes est **fondamental en IT et cybersécurité**

---

## 🔹 Système Binaire (Base 2)

### 📌 Définition
Le système binaire utilise uniquement **deux chiffres** :
- **0** → absence de signal
- **1** → présence de signal

C’est la base fondamentale du fonctionnement des ordinateurs.

### 📘 Terminologie
- **Bit** : un chiffre binaire (0 ou 1)
- **Nibble** : 4 bits
- **Octet (Byte)** : 8 bits

Exemple :
Exemple :
1 octet = 10101010


### 🛠️ Applications en informatique
- Adresses IP et masques de sous-réseau
- Adresses MAC
- Permissions de fichiers
- Encodage des caractères
- Données stockées en mémoire

---

### 🔄 Conversion Binaire → Décimal
1011₂
= (1×2³) + (0×2²) + (1×2¹) + (1×2⁰)
= 8 + 0 + 2 + 1
= 11₁₀


---

## 🔹 Système Octal (Base 8)

### 📌 Définition
Le système octal utilise les chiffres de **0 à 7**.

Chaque chiffre octal représente **3 bits binaires**.

Exemple :
7₈ = 111₂


### 🐧 Utilisation principale : Linux / Unix
Le système octal est utilisé pour gérer les **permissions de fichiers**.

### 🔐 Permissions Linux
Chaque permission a une valeur :
- **Lecture (r)** = 4
- **Écriture (w)** = 2
- **Exécution (x)** = 1

### 📊 Exemples courants
755 = rwxr-xr-x
644 = rw-r--r--


### 🧪 Commande pratique
chmod 755 nom_fichier


👉 Le propriétaire a tous les droits, les autres seulement lecture/exécution.

---

## 🔹 Système Décimal (Base 10)

### 📌 Définition
C’est le système utilisé par les humains.
Il utilise **10 chiffres (0 à 9)**.

### 📍 Utilisation en informatique
- Interfaces utilisateur
- Numéros de ports (80, 443, 22…)
- Valeurs de configuration
- Adressage IP en notation décimale pointée

Exemple :
192.168.1.1


---

## 🔹 Système Hexadécimal (Base 16)

### 📌 Définition
Le système hexadécimal utilise :
- Chiffres : 0 à 9
- Lettres : A à F
  - A = 10, B = 11, … F = 15

### 🔗 Relation avec le binaire
Chaque chiffre hexadécimal = **4 bits**

Exemple :
F = 1111

### 🛠️ Applications IT
- Adresses mémoire
- Codes couleur CSS : #FF0000
- Adresses MAC
- Adresses IPv6
- Valeurs de hachage (MD5, SHA)

### 🔄 Exemple MAC (Hexa → Binaire)
00:1A:2B:3C:4D:5E
00000000:00011010:00101011:00111100:01001101:01011110


---

## 🔤 Encodage de Caractères

### 🅰️ ASCII
- Standard **7 bits**
- 128 caractères
- Lettres, chiffres, ponctuation de base

Exemple :
A = 65 (décimal)

---

### 🌍 Unicode (UTF-8 / UTF-16)
- Standard universel
- Supporte **toutes les langues**
- Compatible avec ASCII
- Utilisé sur le web (HTML, JSON, XML)

👉 UTF-8 est le standard le plus utilisé.

---

### 🔐 Base64
Encodage qui transforme les données binaires
en texte lisible ASCII.

### 📌 Utilisations
- Pièces jointes email
- API Web
- Certificats SSL/TLS
- Jetons JWT

⚠️ Base64 **n’est pas du chiffrement**, فقط encodage.

---

## 🧩 Résumé Rapide

| Système | Base | Utilisation principale |
|-------|------|-----------------------|
| Binaire | 2 | Fonctionnement machine |
| Octal | 8 | Permissions Linux |
| Décimal | 10 | Utilisation humaine |
| Hexadécimal | 16 | Réseau, mémoire |
| ASCII | - | Texte basique |
| Unicode | - | Toutes langues |
| Base64 | - | Données web |

---

## 🎯 Conclusion
Les systèmes de numération sont la base de toute l’informatique.
Les maîtriser permet de mieux comprendre :
- Les réseaux
- Les systèmes
- La cybersécurité
- Le fonctionnement interne des machines
