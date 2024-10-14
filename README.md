<p align="right">
  [English]
  [<a href="README-ko.md">한국어</a>]
</p>

# BooxResizer

BooxResizer is a Python script that resizes and crops images to fit the resolution of Onyx Boox e-readers.

> The script is currently optimized for popular Onyx Boox models and will support all Onyx Boox models in the future.

### Onyx Boox

- Go 10.3 (2480x1860)
- Tab X (1650×2200)
- Page (1264x1680)
- Note Air 2 Plus (1404x1872 )
- Go 6 (1072×1448)
- Palma (824x1648)
- Go Color 7 (1264x1680)
- Note Air 3 C (2480x1860)
- Tab Ultra C Pro (2480x1860)
- Tab Mini C (1872x1404)

### Features

- Process a single image or an entire directory at once
- Supports interactive mode for easy, guided usage
- Supports image formats: `jpg`, `jpeg`, `png`

<img width="682" alt="ss" src="https://github.com/user-attachments/assets/2c593a12-eb98-4d0d-a115-22089b6d40be">

### Installation

Clone the project:

```bash
git clone https://github.com/micronzone/BooxResizer.git
cd BooxResizer
```

Grant execute permissions:
```bash
chmod +x booxresizer
```

Optional: Add an alias for easier use:

```bash
nano ~/.zshrc   # macOS ~/.zshrc, Linux `~/.bashrc` or `~/.zshrc`
alias booxresizer='/path/to/booxresizer'
```

```bash
source ~/.zshrc
```

### Dependencies

FFmpeg can be downloaded from the [official website](https://ffmpeg.org/download.html)

For macOS, you can install it with:
```bash
brew install ffmpeg
```

### Usage

BooxResizer can be used via the command line interface (CLI) or in interactive mode.

```bash
# If you added an alias for booxresizer (see installation) or run it directly from the BooxResizer directory:
booxresizer
booxresizer [file or directory]
```

### Examples

Convert a single image from the wallpaper directory:
```bash
booxresizer ~/Wallpapers/cat.png
```

Batch convert all images in the wallpaper directory:
```bash
booxresizer ~/Wallpapers
```

### Updates

It's a good idea to check for updates to the BooxResizer repository!

```sh
cd BooxResizer
git status
```

To pull the latest changes:

```sh
git pull origin main
```

### License

This project is licensed under the MIT License. For more details, see the [LICENSE](LICENSE) file.

Let me know if you'd like to make any further adjustments!