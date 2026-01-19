# 🔢 Systèmes de Numération en Informatique

<img width="2056" height="1040" alt="Number_System" src="https://github.com/user-attachments/assets/b220a987-d7c3-4f70-a701-9aacf5752188" />

Les systèmes de numération sont des méthodes utilisées pour représenter
les nombres. En informatique, ils sont essentiels car les ordinateurs
ne comprennent que les signaux électriques (0 et 1).

---

## 🧠 Pourquoi les systèmes de numération sont importants ?

- L’ordinateur fonctionne uniquement en **binaire**.
- Les réseaux, la sécurité et les systèmes utilisent différentes bases
  pour simplifier la lecture et la gestion.
- Comprendre ces systèmes est **fondamental en IT et cybersécurité**.
- Permet d'interpréter les données, configurer les adresses IP, les
  permissions Linux, et les codes couleur ou adresses mémoire.

---

## 🔹 Système Binaire (Base 2)

### 📌 Définition
Le système binaire utilise uniquement **deux chiffres** :
- **0** → absence de signal électrique.
- **1** → présence de signal électrique.  

C’est la base fondamentale du fonctionnement des ordinateurs, car
tout le matériel traite des signaux électriques ON/OFF.

### 📘 Terminologie
- **Bit** : un chiffre binaire (0 ou 1).  
- **Nibble** : 4 bits (demi-octet).  
- **Octet (Byte)** : 8 bits, unité standard pour représenter une donnée.

### 📎 Exemple
1 octet = 10101010



### 🛠️ Applications en informatique
- Adresses IP et masques de sous-réseau.  
- Adresses MAC.  
- Permissions de fichiers (binaire → octal).  
- Encodage des caractères (ASCII, Unicode).  
- Données stockées en mémoire vive et sur disque.
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
Le système octal est surtout utilisé pour gérer les **permissions des fichiers**.

### 🔐 Permissions Linux
Chaque permission a une valeur :
- **Lecture (r)** = 4  
- **Écriture (w)** = 2  
- **Exécution (x)** = 1  

### 📊 Exemples courants
755 = rwxr-xr-x (propriétaire: tous droits, groupe: lecture/exécution, autres: lecture/exécution)

644 = rw-r--r-- (propriétaire: lecture/écriture, groupe: lecture, autres: lecture)

### 🧪 Commande pratique
chmod 755 nom_fichier



👉 Le propriétaire a tous les droits, les autres seulement lecture/exécution.

---

## 🔹 Système Décimal (Base 10)

### 📌 Définition
Système naturel utilisé par les humains, avec **10 chiffres (0 à 9)**.

### 📍 Utilisation en informatique
- Interfaces utilisateur.  
- Numéros de ports réseau (HTTP=80, HTTPS=443, SSH=22…).  
- Valeurs de configuration dans les logiciels.  
- Adressage IP en notation décimale pointée.

### 📎 Exemple

192.168.1.1

---


## 🔹 Système Hexadécimal (Base 16)

### 📌 Définition
Le système hexadécimal utilise :
- Chiffres : 0 à 9  
- Lettres : A à F  
  - A = 10, B = 11, … F = 15

### 🔗 Relation avec le binaire
Chaque chiffre hexadécimal correspond à **4 bits binaires**.

### 📎 Exemple
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

Une adresse MAC est composée de **6 octets**, chacun représenté par **2 caractères hexadécimaux**.

| Octet Hexa | Décimal | Binaire  |
| ---------- | ------- | -------- |
| 00         | 0       | 00000000 |
| 1A         | 26      | 00011010 |
| 2B         | 43      | 00101011 |
| 3C         | 60      | 00111100 |
| 4D         | 77      | 01001101 |
| 5E         | 94      | 01011110 |

---

### 🔹 Étape par étape pour convertir chaque octet

1. **00 (hex)** → decimal = 0

   * 0 en binaire = `00000000` (8 bits)

2. **1A (hex)** → decimal = 26

   * 1A en hex = (1 × 16) + (A × 1)
   * A = 10 → 1 × 16 + 10 = 26
   * 26 en binaire = `00011010`

3. **2B (hex)** → decimal = 43

   * 2B = (2 × 16) + (B × 1)
   * B = 11 → 2 × 16 + 11 = 43
   * 43 en binaire = `00101011`

4. **3C (hex)** → decimal = 60

   * 3C = (3 × 16) + (C × 1)
   * C = 12 → 3 × 16 + 12 = 60
   * 60 en binaire = `00111100`

5. **4D (hex)** → decimal = 77

   * 4D = (4 × 16) + (D × 1)
   * D = 13 → 4 × 16 + 13 = 77
   * 77 en binaire = `01001101`

6. **5E (hex)** → decimal = 94

   * 5E = (5 × 16) + (E × 1)
   * E = 14 → 5 × 16 + 14 = 94
   * 94 en binaire = `01011110`

---

### 🔹 Résultat final

```
00:1A:2B:3C:4D:5E
=
00000000:00011010:00101011:00111100:01001101:01011110
```

Chaque **octet hexadécimal** est maintenant **8 bits binaires**, séparés par `:` pour correspondre à l’adresse MAC complète.

---

💡 **Astuce pour retenir** :

* Hexadécimal → Binaire : chaque chiffre hex = **4 bits**.
* 2 chiffres hex = 1 octet = 8 bits.
* On convertit chaque chiffre séparément ou ensemble pour obtenir 8 bits.
---

## 🔤 Encodage de Caractères

### 🅰️ ASCII
ASCII = **American Standard Code for Information Interchange**
* Chaque caractère a **un code numérique** compris entre 0 et 127 (7 bits).
* Les caractères incluent : lettres (A-Z, a-z), chiffres (0-9), ponctuation, et quelques commandes de contrôle.


Exemple :
A = 65 (décimal)

### 🔹 Étape par étape pour A

1. **Identifier le caractère** :

   * On prend **A** (lettre majuscule)

2. **Vérifier la table ASCII** :

   * Les lettres majuscules sont codées de 65 à 90.
   * Donc :

     ```
     A = 65
     B = 66
     C = 67
     ...
     Z = 90
     ```

3. **Conversion en binaire (7 bits)** :

   * 65 en décimal → convertir en binaire :

     ```
     65 ÷ 2 = 32 reste 1
     32 ÷ 2 = 16 reste 0
     16 ÷ 2 = 8 reste 0
     8 ÷ 2 = 4 reste 0
     4 ÷ 2 = 2 reste 0
     2 ÷ 2 = 1 reste 0
     1 ÷ 2 = 0 reste 1
     ```
   * En lisant les restes du bas vers le haut : `1000001`
   * Donc :

     ```
     A = 65 décimal = 1000001 binaire (7 bits)
     ```

4. **Vérification** :

   * 7 bits → 2⁶ + 0 + 0 + 0 + 0 + 0 + 1 = 64 + 1 = 65 

---

### 🔹 Résumé

| Caractère | Décimal | Binaire 7 bits |
| --------- | ------- | -------------- |
| A         | 65      | 1000001        |

---

💡 **Astuce** :

* Majuscules = 65 → 90
* Minuscules = 97 → 122
* Chiffres = 48 → 57

---

### 🌍 Unicode (UTF-8 / UTF-16)
- Standard universel  
- Supporte toutes les langues  
- Compatible ASCII  
- Utilisé sur le web (HTML, JSON, XML)  

👉 **UTF-8** est le standard le plus utilisé pour le texte web.

---

### 🔐 Base64
- Transforme les données binaires en **texte ASCII lisible**.  
- **Applications** : pièces jointes email, API Web, certificats SSL/TLS, jetons JWT.  

⚠️ Base64 **n’est pas un chiffrement**, seulement un encodage.

---

## 🧩 Résumé Rapide

| Système | Base | Utilisation principale |
|-------|------|-----------------------|
| Binaire | 2 | Fonctionnement machine, données mémoire |
| Octal | 8 | Permissions Linux / Unix |
| Décimal | 10 | Utilisation humaine, interfaces |
| Hexadécimal | 16 | Réseau, mémoire, codes couleur |
| ASCII | - | Texte basique |
| Unicode | - | Toutes langues |
| Base64 | - | Données web, emails, API |

---

## 🎯 Conclusion
Les systèmes de numération sont la **base de toute l’informatique**.  
Les maîtriser permet de mieux comprendre :
- Les réseaux et adresses IP / MAC  
- Les systèmes et permissions  
- La cybersécurité  
- Le fonctionnement interne des ordinateurs
