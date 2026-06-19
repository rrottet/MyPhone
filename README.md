# ✅ Mes tâches — To-do list pour Samsung

Une petite to-do list **sans installation**, qui fonctionne **hors-ligne** dans le
navigateur de ton téléphone Samsung (Chrome ou Samsung Internet).

## Fonctionnalités
- Ajouter une tâche
- Cocher / décocher
- Supprimer
- Sauvegarde automatique sur le téléphone (rien n'est envoyé sur internet)
- Installable sur l'écran d'accueil (comme une vraie appli)

## Comment l'essayer sur le Samsung

### Option simple (ouvrir le fichier)
1. Copie le dossier sur ton téléphone (câble USB, Google Drive, etc.)
2. Ouvre `index.html` avec **Chrome** ou **Samsung Internet**

### Option recommandée (vrai test PWA, hors-ligne + installation)
Le mode hors-ligne et l'installation nécessitent un petit serveur web.
Depuis un ordinateur sur le **même Wi-Fi** que le téléphone :

```bash
# Dans ce dossier
python3 -m http.server 8000
```

Puis sur le téléphone, ouvre :
```
http://IP-DE-TON-ORDI:8000
```
(remplace `IP-DE-TON-ORDI` par l'adresse IP locale du PC)

Dans le menu du navigateur Samsung → **« Ajouter la page à »** → **Écran d'accueil**
pour l'installer comme une appli.

## Fichiers
| Fichier | Rôle |
|---------|------|
| `index.html` | L'application complète (HTML + CSS + JS) |
| `manifest.webmanifest` | Métadonnées PWA (nom, couleurs, icône) |
| `sw.js` | Service worker (fonctionnement hors-ligne) |
| `icon.svg` | Icône de l'application |
