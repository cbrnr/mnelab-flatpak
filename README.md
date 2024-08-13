## MNELAB Flatpak

This repository contains the files needed to build a flatpak for [MNELAB](https://github.com/cbrnr/mnelab). Note that this is work in progress and the flatpak is not yet available on Flathub.


### Building

To build the flatpak, you need to have `flatpak` and `flatpak-builder` installed (https://flatpak.org/setup/). You also need to have the `flathub` remote added to your installation.

To build the MNELAB flatpak, run the following command:

```bash
flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir io.github.mnelab.MNELAB.yaml
```


### Running

Running the installed flatpak is as simple as running the following command:

```bash
flatpak run io.github.mnelab.MNELAB
```


### Background information

- https://docs.flatpak.org/en/latest/conventions.html
- https://docs.flathub.org/docs/for-app-authors/metainfo-guidelines/
- https://docs.flathub.org/docs/for-app-authors/metainfo-guidelines/quality-guidelines
