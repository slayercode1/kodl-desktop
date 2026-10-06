<p align="center">
  <img src="https://kodl.fr/kodl-icon-120.png" alt="Kodl" width="96" height="96" />
</p>

<h1 align="center">Kodl pour ordinateur</h1>

<p align="center">
  La gestion de projet simple pour toutes les équipes : tâches, sprints, chat, appels et documentation au même endroit.<br />
  <a href="https://kodl.fr/download"><strong>Télécharger Kodl</strong></a> ·
  <a href="https://kodl.fr">kodl.fr</a> ·
  <a href="#english">English</a>
</p>

---

## Télécharger

Le plus simple : **[kodl.fr/download](https://kodl.fr/download)** détecte votre système et propose le bon fichier.

Vous pouvez aussi prendre les fichiers dans la [dernière version](../../releases/latest) :

| Système | Fichier | Pour qui |
|---|---|---|
| **Windows** 10 ou 11, 64 bits | `Kodl_<version>_x64-setup.exe` | Recommandé, installation sans droits administrateur |
| | `Kodl_<version>_x64_en-US.msi` | Déploiement géré par un service informatique |
| **macOS** 11 Big Sur ou plus récent | `Kodl_<version>_universal.dmg` | Mac Apple Silicon et Intel |
| **Linux** 64 bits | `Kodl_<version>_amd64.AppImage` | Recommandé, toutes distributions |
| | `Kodl_<version>_amd64.deb` | Debian, Ubuntu, Linux Mint |
| | `Kodl-<version>-1.x86_64.rpm` | Fedora, openSUSE, Rocky Linux |

L’app de bureau est **gratuite**, incluse dans tous les plans : c’est le même Kodl, avec le même compte.

## Ce que l’app ajoute

- 🔔 **Notifications natives** : mentions, messages et appels, même fenêtre fermée.
- 🔴 **Non-lus en un coup d’œil** dans la barre des tâches ou le Dock.
- 🚀 **Toujours à portée** : lancement à l’ouverture de session et zone de notification.
- 🔗 **Liens qui ouvrent l’app** : les liens Kodl reçus par e-mail s’ouvrent dans la fenêtre de Kodl.
- 🔐 **Session protégée** : connexion par votre navigateur habituel, session rangée dans le trousseau du système.
- 📴 **Utilisable hors ligne** pour les pages déjà consultées.

## Première ouverture

Les installeurs ne sont pas encore signés par un certificat d’éditeur : votre système demande une confirmation **une seule fois**. Téléchargez Kodl uniquement depuis [kodl.fr/download](https://kodl.fr/download) ou depuis ce dépôt.

<details>
<summary><strong>Windows</strong></summary>

1. Si votre navigateur signale un fichier peu téléchargé, choisissez de le **conserver**.
2. Ouvrez l’installeur. Si Windows affiche « Windows a protégé votre ordinateur », cliquez sur **Informations complémentaires**.
3. Cliquez sur **Exécuter quand même**.
</details>

<details>
<summary><strong>macOS</strong></summary>

1. Ouvrez l’image disque et glissez Kodl dans **Applications**.
2. Ouvrez Kodl. macOS indique qu’il ne peut pas vérifier l’app : fermez ce message.
3. Dans **Réglages Système › Confidentialité et sécurité**, cliquez sur **Ouvrir quand même**, puis confirmez.
</details>

<details>
<summary><strong>Linux</strong></summary>

- **AppImage** : rendez le fichier exécutable (clic droit › Propriétés › Autoriser l’exécution, ou `chmod +x Kodl_*.AppImage`), puis ouvrez-le.
- **.deb / .rpm** : ouvrez-le avec votre gestionnaire de logiciels, ou :
  ```bash
  sudo apt install ./Kodl_*_amd64.deb      # Debian, Ubuntu
  sudo dnf install ./Kodl-*.x86_64.rpm     # Fedora
  ```
</details>

## Vérifier un téléchargement

Chaque version publie un fichier `SHA256SUMS`. Placez-le à côté de votre installeur, puis :

```bash
# Linux
sha256sum --check --ignore-missing SHA256SUMS
# macOS
shasum -a 256 --check --ignore-missing SHA256SUMS
```

```powershell
# Windows (PowerShell) : comparez avec la ligne correspondante de SHA256SUMS
Get-FileHash .\Kodl_*_x64-setup.exe -Algorithm SHA256
```

## Mises à jour

L’interface de Kodl est chargée depuis kodl.fr : vous avez toujours les dernières fonctionnalités. Seule la fenêtre de l’app (notifications, icônes) se met à jour en installant une nouvelle version d’ici.

## Contact

Ce dépôt sert uniquement à distribuer les installeurs ; le code source de Kodl n’y est pas publié.
Une question, un problème ou une faille de sécurité à signaler : **contact@kodl.fr**.

---

<h2 id="english">English</h2>

**Kodl for desktop**: simple project management for every team. Tasks, sprints, chat, calls and documentation in one place.

### Download

Easiest: **[kodl.fr/en/download](https://kodl.fr/en/download)** detects your system and offers the right file. The files are also in the [latest release](../../releases/latest):

| System | File |
|---|---|
| **Windows** 10 or 11, 64-bit | `Kodl_<version>_x64-setup.exe` (recommended) or `.msi` (IT-managed deployment) |
| **macOS** 11 Big Sur or later | `Kodl_<version>_universal.dmg` (Apple silicon and Intel) |
| **Linux** 64-bit | `.AppImage` (recommended), `.deb` or `.rpm` |

The desktop app is **free** and included in every plan: same Kodl, same account.

### First launch

The installers are not signed with a publisher certificate yet, so your system asks you to confirm **once**. Only download Kodl from [kodl.fr/en/download](https://kodl.fr/en/download) or this repository.

- **Windows**: if SmartScreen shows “Windows protected your PC”, click **More info**, then **Run anyway**.
- **macOS**: open Kodl once, close the warning, then go to **System Settings › Privacy & Security** and click **Open Anyway**.
- **Linux**: make the AppImage executable (`chmod +x Kodl_*.AppImage`), or install the `.deb` / `.rpm` with your package manager.

### Verify a download

Each release ships a `SHA256SUMS` file: run `sha256sum --check --ignore-missing SHA256SUMS` (Linux), `shasum -a 256 --check --ignore-missing SHA256SUMS` (macOS) or `Get-FileHash <file> -Algorithm SHA256` (Windows).

### Contact

This repository only distributes the installers; Kodl’s source code is not published here. Questions, issues or security reports: **contact@kodl.fr**.
