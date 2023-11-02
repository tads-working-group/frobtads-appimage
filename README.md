# frobtads-appimage

This repository provides self-contained distro-agnostic AppImages of the
`t3make` (TADS 3 compiler) and `frob` (terminal interpreter) executables
provided by the FrobTADS project, so as to make them much easier to install on
Linux, since you will no longer need to build them from source.

This repository also contains an "Author's Kit" for Linux, distributed as a ZIP
file, which provides:

- the TADS 3 compiler (t3make)
- the TADS 2/3 terminal interpreter/runner (frob)
- the TADS 3 system libraries (including adv3)
- the alternative standard library, adv3lite

## Installing just the executables

To install just the bare executable appimages, follow these three steps:

1. Go to the Releases page in the right sidebar of this GitHub project and
   download the `frob-x86_64.AppImage` and `t3make-x86_64.AppImage` files
2. Run `chmod +x` on both files in the terminal to make them executable
3. Move them to somewhere in your shell's PATH, such as
   `/usr/local/bin/` or, preferably, `$HOME/.local/bin/`

After installation, you'll be able to use the frob command by running:

```bash
$ frob-x86_64.AppImage myGameFile.t3
```

and the t3make compiler by running:

```bash
$ # in a valid TADS 3 project
$ t3make-x86_64.AppImage
```

## Installing the full "Author's Kit" distribution

To install the full distribution, follow these steps:

1. Go to the Releases page on the right sidebar of this GitHub project and
   download `authors-kit.zip`
2. Unzip the folder
3. follow the steps in the previous section regarding the two appimages
4. then move the `tads3/` folder wherevery you want, probably to your home
   directory
4. Point your t3m file's `-FI` and `-FL` directeves at the relevant
   `tads3/include` and `tads3/lib` directories wherever you moved the `tads3/`
   folder
