## MNELAB Flatpak

This repository contains the files needed to build a flatpak for [MNELAB](https://github.com/cbrnr/mnelab).


### Building

To build the Flatpak, you need to have flatpak and flatpak-builder installed (https://flatpak.org/setup/). You also need to have the flathub remote added to your flatpak installation.

```bash
flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir io.github.mnelab.MNELAB.yaml
```


### Running

Running the installed Flatpak is as simple as running the following command:

```bash
flatpak run io.github.mnelab.MNELAB
```


### Background information

https://docs.flatpak.org/en/latest/conventions.html
https://docs.flathub.org/docs/for-app-authors/metainfo-guidelines/
https://docs.flathub.org/docs/for-app-authors/metainfo-guidelines/quality-guidelines
