## Files

`/clove` contains all the images I use actively

`/girls` contains all the code for [Girls Discord](https://discord.gg/TransRights)

## Commands
To convert the SVGs to PNGs, I used the below:
```bash
brew install inkscape # MacOS
sudo apt install inkscape # Debian/Ubuntu
sudo pacman -S inkscape # Arch
sudo dnf install inkscape # Fedora
# Windows: download the latest .msi installer from the Inkscape website

for f in ./svg/*.svg; do
  filename=$(basename "$f" .svg)
  inkscape "$f" --export-type=png --export-background-opacity=0 --export-filename="./png/$filename.png"
done
```

---

<sub>The MIT license in this repository applies only to the source code authored by the repository owner. Third-party marks referenced in `clove/svg/archian.svg` and `clove/svg/archian-spanner.svg` are the property of their respective projects and are not covered by the MIT license. The Debian swirl is a trademark of Software in the Public Interest, Inc., used under the [Debian Open Use Logo License](https://www.debian.org/logos/). The Arch Linux logo is a trademark of the Arch Linux project; the recolored derivative used here is for personal, non-commercial identification purposes per the [Arch Linux trademark guidelines](https://archlinux.org/art/). No endorsement or affiliation with either project is implied.</sub>