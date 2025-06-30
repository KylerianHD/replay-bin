# replay-bin

AUR package for [Replay by Weights](https://www.weights.com/replay) - AI Audio Tool for generating songs, voice covers, and more.

## Description

Replay is a desktop application that allows you to create AI music covers, text to speech, and train your own RVC model. It is offline, local, and free. This repository aims to provide Replay via the AUR.

### Key Features of Replay

- **AI Voice Covers**: Transform any song by changing the vocalist to any voice model from a voice library
- **Text-to-Speech**: Convert text into natural-sounding speech using various AI voice models
- **Speech Conversion**: Transform speech recordings into different voices
- **RVC Training**: Train your own Retrieval-based Voice Conversion models
- **Multimodel Voice Fusion**: Blend multiple voices in a single track or switch between them

## Installation

### From AUR using an AUR helper

Using yay:
```bash
yay -S replay-bin
```

Using paru:
```bash
paru -S replay-bin
```

### Manual installation

```bash
git clone https://github.com/KylerianHD/replay-bin.git
cd replay-bin
makepkg -si
```

## Usage

After the installation, you can launch Replay from your application menu or by running:

```bash
replay
```

Keep in mind that you will need a Weights account in Order to use/access Replay.

### Getting Started

1. **Launch Replay**: Start Replay
2. **Connect to Weights**: Log in or sign up to your Weights account 
3. **Select Your Task**:
   - **Vocal Conversion**: Select a song and a voice model to create a cover
   - **Stem Audio**: Separate stems from an audio file
   - **Train Model**: Create your own custom voice model using RVC training
   - **Sample Generation (early testing)**: Lets you generate samples from audio and lyrics

### Voice Models

Replay works with voice models from Weights or other platforms. You can:
- Use pre-trained models
- Train your own custom voice models

## System Requirements & Troubleshooting

Obviously, you need good enough hardware to use Replay, but I can say from my own experience that it works very well on an NVIDIA GTX 1660 Ti and with around 16GB of RAM. However, more is definitely better. I use Arch with KDE Plasma and Wayland and haven't had any issues, so feel free to open an issue if you encounter any problems.

## Links

- **Weights Website**: [weights.com](https://www.weights.com)
- **Weights/Replay Discord**: [discord.gg/weights](https://discord.gg/weights) 
- **Weights/Replay Reddit**: [reddit.com/r/weights](https://reddit.com/r/weights)

## License

This AUR package follows the licensing of Replay by Weights. However, because the license isn't clear (even the original application on Debian and Windows has the license set to "unknown"), I set it to GPL-V3 and "unknown" too. If you are from the Weights/Replay team, please contact me if there are any issues regarding the license.

## Contributing

To contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add some improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a new Pull Request

Or create an issue/discussion with the appropriate tag.

## Maintainer

- **AUR Package Maintainer**: KylerianHD
- **Upstream**: [Weights.com](https://www.weights.com/replay)

## Disclaimer

This is an unofficial AUR package for Replay by Weights. All trademarks and software belong to their respective owners.

---

If you find this package useful, please vote for it on the AUR!
