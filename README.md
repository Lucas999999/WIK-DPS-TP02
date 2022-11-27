# WIK-DPS-TP01

Voici le rendu du TP 1 de devops, le but de ce tp était de faire une API qui retourne les headers d'un requête effectuée sur la route /ping et une réponse avec un code 404 sur les autres routes, j'ai fait cette API en rust, voici les instructions d'utilisation:

## Instructions
### Installation

Tout d'abord il faut cloner ce repertoire git là où on veut:

```
git clone https://github.com/Lucas999999/WIK-DPS-TP01.git
```

Ensuite il nous faut cargo, le gestionnaire de paquets de Rust, c'est le plus simple pour lancer le projet.
voici la doc de [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html).

Sur linux:

```
curl https://sh.rustup.rs -sSf | sh
```
Sur windows:

[rustup-init.exe](https://win.rustup.rs/)

Ou alors avec votre gestionnaire de paquets préféré.
### Utilisation

Maintenant que nous avons tout ce qu'il faut il ne reste plus qu'à lancer le projet, c'est la partie la plus simple, il suffit de taper:

```
cargo run
```

on peut également préciser un port sur lequel le serveur va écouter (le port de base est 3333) pour cela il faut définir une variable d'environnement "PING_LISTEN_PORT" qui a pour valeur le port voulu.

Pour créer une variable d'environnement:

sur linux:

```
export PING_LISTEN_PORT=4444
```

sur windows:

```
$env:PING_LISTEN_PORT = '4444'
```