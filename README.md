# 🐍 SERPENT.EXE — Version 1.0

> Application mobile de jeu Snake développée en Flutter/Dart.

---

## 📱 Présentation de l'application

SERPENT.EXE est un jeu Snake moderne avec une esthétique néon cyberpunk.
Le joueur contrôle un serpent qui grandit en mangeant de la nourriture.
Plus le serpent mange, plus il grandit et plus le jeu devient difficile.
Le but est d'obtenir le meilleur score possible sans se mordre la queue.

---

## ✨ Fonctionnalités

### 🎮 Jeu
- Serpent contrôlable avec le D-Pad ou les touches fléchées du clavier
- La nourriture apparaît aléatoirement sur la grille
- Le serpent grandit à chaque nourriture mangée
- Nourriture bonus (étoile violette) qui rapporte 50 points et disparaît après quelques secondes
- Système de téléportation : le serpent traverse les bords et réapparaît de l'autre côté

### 🏆 Score et niveaux
- Chaque nourriture rapporte des points selon la difficulté choisie
- Le niveau augmente tous les 5 nourritures mangées
- La vitesse du serpent augmente avec le niveau
- Affichage du meilleur score de la session

### ⚙️ Difficultés
- **EASY** — Vitesse lente, multiplicateur x1
- **NORMAL** — Vitesse normale, multiplicateur x2
- **HARD** — Vitesse rapide, multiplicateur x3
- **INSANE** — Vitesse très rapide, multiplicateur x5

### 🎨 Thèmes graphiques
- **Thème Sombre** — Fond noir avec effets néon colorés
- **Thème Clair** — Fond lavande avec serpent rose

### 🎵 Sons
- Musique d'ambiance sur le menu
- Musique différente pendant le jeu
- Son spécial au Game Over

### ⏸️ Pause
- Possibilité de mettre le jeu en pause à tout moment
- Reprendre la partie là où on s'est arrêté

---

## 🛠️ Technologies utilisées

- **Flutter** — Framework de développement mobile
- **Dart** — Langage de programmation
- **audioplayers** — Gestion des sons et musiques

---

## 📁 Structure du projet

```
snake_buggy/
├── lib/
│   └── main.dart        ← Code source principal
├── assets/
│   └── audio/
│       ├── menu.mp3     ← Musique du menu
│       ├── game.mp3     ← Musique du jeu
│       └── gameover.mp3 ← Musique game over
└── pubspec.yaml         ← Dépendances du projet
```

---

## 🚀 Lancer l'application

```bash
flutter pub get
flutter run -d chrome --web-renderer html
```

---

*Version 1.0 — stable*

