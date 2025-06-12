# 🖨️ ft_printf

Bienvenue sur **ft_printf** !  
Une ré-implémentation personnalisée de la fameuse fonction `printf` de la bibliothèque standard C, dans le cadre du cursus 42.  
Ce projet vous permet de mieux comprendre la gestion des arguments variadiques, le parsing et l'affichage formaté en C.  

---

## 🚀 Fonctionnalités

- ⚡ Réimplémente les conversions principales de `printf`
- ✍️ Gestion des types de base
- 🛑 Gestion des cas particuliers (null, pointeur nul, etc.)
- 🎯 Retourne le nombre de caractères affichés

---

## 🛠️ Types et conversions supportés

| Spécificateur | Signification              | Exemple d’appel                  | Résultat attendu      |
|:-------------:|:--------------------------|:---------------------------------|:----------------------|
| `%c`          | Caractère                 | `ft_printf("%c", 'A');`          | A                    |
| `%s`          | Chaîne de caractères      | `ft_printf("%s", "Hello");`      | Hello                |
| `%d` ou `%i`  | Entier signé              | `ft_printf("%d", 42);`           | 42                   |
| `%u`          | Entier non signé          | `ft_printf("%u", 42);`           | 42                   |
| `%x`          | Hexa minuscule            | `ft_printf("%x", 255);`          | ff                   |
| `%X`          | Hexa majuscule            | `ft_printf("%X", 255);`          | FF                   |
| `%p`          | Pointeur                  | `ft_printf("%p", ptr);`          | 0x16fd6b804          |
| `%%`          | Pourcentage littéral      | `ft_printf("%%");`               | %                    |

---

## 🧩 Utilisation

### 1. Compilation

```bash
cd printf
make
```
Cela va générer la librairie statique `libftprintf.a` 🏗️


## 💡 Astuces & Cas particuliers

- Si une chaîne est `NULL`, l'affichage sera `(null)` (conforme à la norme).
- Un pointeur NULL affiche `0x0`.
- Pour `%d`, la valeur minimale d’un int signé est gérée (`-2147483648`).

---

## 📂 Arborescence principale

```
printf/
├── ft_printf.c
├── ft_printf.h
├── ft_print_char.c
├── ft_print_nbr.c
├── ft_print_ptr.c
├── ft_print_str.c
├── ft_print_u_nbr.c
├── ft_print_x_nbr.c
├── Makefile
└── libftprintf.a
```

---

## 🤝 Contribution

Les contributions sont les bienvenues !  
N'hésitez pas à cloner, forker et proposer vos améliorations via des pull requests.  

---

## 🧑‍💻 Auteur

- [chaymae-bayousfi](https://github.com/chaymae-bayousfi)  

---

## 📜 Licence

Ce projet est sous licence MIT.  
Faites-en bon usage et amusez-vous ! 🚀

---
