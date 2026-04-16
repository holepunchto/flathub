# Keet Flatpak

Github repo for the [Keet](https://keet.io) Flatpak.

## Install the Flatpak dependency

```sh
$ sudo apt install flatpak
$ flatpak remote-add --if-not-exists --user flathub https://dl.flathub.org/repo/flathub.flatpakrepo
$ flatpak install flathub org.flatpak.Builder
```

## Install the Keet Flatpak

```
$ git clone git@github.com:holepunchto/flathub.git
$ git checkout keet-app-submission
$ flatpak run --command=flathub-build org.flatpak.Builder --disable-rofiles-fuse io.keet.Keet.yml
$ flatpak install --user ./repo io.keet.Keet
```

## Run

Using GUI: search Keet and run it

Or use CLI:

```
$ flatpak run io.keet.Keet
```

## Uninstall:

```
$ flatpak uninstall io.keet.Keet
```
