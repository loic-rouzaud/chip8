# Chip8 Emulateur

**CHIP-8** est un langage de programmation hexadécimal interprété utilisant une machine virtuelle
développé par Joseph Weisbecker en 1978. Il était spécifiquement conçu pour faciliter la conception
de jeux vidéo sur les micro-ordinateurs 8-bits bas de gamme de cette époque.

## opcodes

Les opcodes (codes d'opération) sont des instructions en langage machine utilisées par la machine virtuelle CHIP-8 pour exécuter des programmes. Chaque opcode est un mot de 16 bits (2 octets) et est généralement représenté en hexadécimal. Voici une description des principaux opcodes utilisés dans CHIP-8 :

Structure des Opcodes

Les opcodes CHIP-8 sont généralement divisés en quatre nibbles (chiffres hexadécimaux), chacun représentant une partie de l'instruction. Par exemple, un opcode 0x1234 peut être décomposé comme suit :

- **Premier nibble (1) :** Représente généralement l'opération principale.
- **Deuxième nibble (2) :** Souvent utilisé pour spécifier des registres ou des adresses.
- **Troisième nibble (3) :** Utilisé pour des valeurs ou des adresses supplémentaires.
- **Quatrième nibble (4) :** Peut également contenir des valeurs ou des adresses.

(voir sources pour mieux comprendre)

# But

Ce projet vise à créer un émulateur CHIP-8 en utilisant le langage de programmation Rust. L'objectif est de fournir une implémentation moderne et efficace de cette machine virtuelle classique, tout en offrant une base pour l'apprentissage et l'expérimentation avec Rust.

# Fonctionnalités

- **Émulation précise** : Implémente fidèlement les instructions CHIP-8.
- **Interface graphique** : Affiche les jeux CHIP-8 avec une interface utilisateur.
- **Support des ROMs** : Chargez et exécutez des fichiers ROM CHIP-8.
- **Performances optimisées** : Utilise les capacités de Rust pour des performances optimales.

# Installation

Pour installer le projet, vous devez avoir Rust et Cargo installés sur votre système. Vous pouvez les installer en suivant les instructions sur le site officiel de Rust : https://www.rust-lang.org/tools/install.

Une fois Rust et Cargo installés, vous pouvez cloner le projet en utilisant la commande suivante :

```bash
git clone git@github.com:loic-rouzaud/chip8.git
```

Ensuite, vous pouvez compiler et exécuter le projet en utilisant les commandes suivantes :
Télécharger les jeux CHIP-8 à partir de https://www.zophar.net/pdroms/chip8/chip-8-games-pack.html

```bash
cd chip8
cargo run <path_to_rom_file>
```

# Contrôles :

Les contrôles par défaut sont configurés pour correspondre aux touches originales CHIP-8. Vous pouvez les modifier dans le fichier de configuration si nécessaire.

(voir sources pour mieux comprendre)

# Sources

https://github.com/aquova/chip8-book/blob/master/src/3-setup.md

https://tobiasvl.github.io/blog/write-a-chip-8-emulator/

https://www.reddit.com/r/EmuDev/comments/128h36t/how_to_decodegetunderstand_or_whatever_chip_8_roms/

https://chip8.gulrak.net/
