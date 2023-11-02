# frobtads-appimage

This repository provides self-contained distro-agnostic AppImages of the
`t3make` (TADS 3 compiler) and `frob` (terminal interpreter) executables
provided by the FrobTADS project, so as to make them much easier to install on
Linux. To install them:

1. go to the Releases page in the right sidebar of this GitHub project and
   download the `frob-x86_64.AppImage` and `t3make-x86_64.AppImage` files,
2. then run `chmod +x` on both files in the terminal to make them executable,
3. and finally, move them to somewhere in your shell's PATH, such as
   `/usr/local/bin/` or, preferably, `$HOME/.local/bin/`.

After installation, you'll be able to use the frob command by running:

```bash
$ frob-x86_64.AppImage myGameFile.t3
```

and the t3make compiler by running:

```bash
$ # in a valid TADS 3 project
$ t3make-x86_64.AppImage
```
