# 🐍 SERPENT.EXE — Version Bêta

> Application mobile de jeu Snake développée en Flutter/Dart .

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

## 🐛 Bugs connus

> Cette version est une version bêta. Les bugs suivants ont été identifiés et sont en cours de correction.

---

### Bug 1 — Le bouton Sombre / Clair ne fonctionne pas
**Ce qui se passe :** Quand on appuie sur le bouton pour changer de thème, rien ne se passe. L'application reste sur le thème sombre même si on clique plusieurs fois.

**Ce qui devrait se passer :** L'application doit basculer entre le thème sombre et le thème clair à chaque appui sur le bouton.

---

### Bug 2 — Les boutons Gauche et Droite du D-Pad sont invisibles
**Ce qui se passe :** Sur l'écran de jeu, seuls les boutons Haut et Bas du D-Pad sont visibles et cliquables. Les boutons Gauche et Droite ont disparu de l'écran.

**Ce qui devrait se passer :** Les 4 boutons directionnels doivent être visibles et permettre de diriger le serpent dans les 4 directions.

---

### Bug 3 — Le bouton JOUER est trop grand
**Ce qui se passe :** Sur l'écran du menu, le bouton JOUER prend toute la largeur de l'écran au lieu d'avoir une taille raisonnable et centrée.

**Ce qui devrait se passer :** Le bouton doit avoir une largeur fixe et être centré sur l'écran comme les autres boutons.

---

### Bug 4 — Aucun son ne se lance
**Ce qui se passe :** Pendant toute l'application (menu, jeu, game over), aucune musique ne se lance. L'application est silencieuse.

**Ce qui devrait se passer :** Une musique doit jouer sur le menu, une autre pendant la partie, et une dernière au Game Over.

---

### Bug 5 — La pause bloque définitivement le jeu
**Ce qui se passe :** Quand on met le jeu en pause, il est impossible de le reprendre. Le bouton "Reprendre" dans l'écran de pause ne fait rien. La seule option est de recommencer une nouvelle partie.

**Ce qui devrait se passer :** Le bouton pause doit alterner entre mettre le jeu en pause et le reprendre là où on s'était arrêté.

---

### Bug 6 — Le serpent peut traverser son propre corps
**Ce qui se passe :** Quand le serpent se retrouve face à son propre corps, il le traverse sans mourir. Le jeu ne s'arrête jamais et le serpent peut passer à travers lui-même indéfiniment.

**Ce qui devrait se passer :** Si la tête du serpent touche son propre corps, la partie doit se terminer et l'écran Game Over doit s'afficher.

---

### Bug 7 — Le score devient négatif
**Ce qui se passe :** À chaque fois que le serpent mange de la nourriture, au lieu de gagner des points, le score diminue et devient négatif.

**Ce qui devrait se passer :** Manger de la nourriture doit augmenter le score du joueur selon la difficulté choisie.

---

### Bug 8 — Le niveau ne monte jamais
**Ce qui se passe :** Peu importe combien de nourritures le serpent mange, le niveau reste bloqué à 1 et la vitesse n'augmente jamais.

**Ce qui devrait se passer :** Tous les 5 nourritures mangées, le niveau doit augmenter d'un et le serpent doit accélérer progressivement.

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

*Version bêta
