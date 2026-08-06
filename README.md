<a id="readme-top"></a>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

<div align="center">
  <h1>Desktop Assistant AI</h1>
  <p>An AI to help users when they don't know what to do, with emphasis on code help.</p>
  <p>
    <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/issues">Report Bug</a>
    ·
    <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/issues">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#built-with">Built With</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About The Project

Desktop-assistant-AI is an AI-powered desktop assistant designed to help users, especially coders, when they are unsure what to do next. It originally intended to take screenshots from PC or screen recording and provide it to the AI for analysis. It is not currently a useful product.

**Platform:** Windows only

### Features

- AI-powered help for coding and general desktop tasks
- Screenshot capture and context-aware assistance
- Integration with OpenAI (ChatGPT) and Whisper for speech recognition
- Text-to-speech responses
- Secure model loading with progress feedback
- Modern PyQt5 GUI

## Getting Started

This project uses a PowerShell script to automate the setup process. It will check for the required Python version (3.11), create a virtual environment, and install all the necessary dependencies.

1. **Download or clone this repository.**

2. **Run the setup script:**

    Open a PowerShell terminal and run the following command:

    ```powershell
    .\setup.ps1
    ```

    The script will guide you through the setup process. If you don't have Python 3.11 installed, it will offer to install it for you from the Microsoft Store.

3. **Run the application:**

    Once the setup is complete, you can launch the application with:

    ```powershell
    .\run.ps1
    ```

**See also:** [gotchas.md](gotchas.md) for troubleshooting common installation issues.

### Developer Setup

To set up a development environment, simply follow the installation instructions above. The `setup.ps1` script will create a self-contained virtual environment in the `.venv` directory, which you can use for development.

### Project Structure

- `src/` — Main source code
- `resources/` — Images and logos
- `run.bat`, `compile.bat` — Windows scripts for running and compiling
- `download_dependencies.sh` — Dependency installer for Linux

## Usage

After installation, launch the assistant using `run.ps1`. The app will show a loading screen while the Whisper and Coqui TTS models load, then present the main window for interaction.

## Built With

- [PyQt5](https://riverbankcomputing.com/software/pyqt/intro) — GUI framework
- [OpenAI](https://openai.com) — ChatGPT and Whisper integration
- [Coqui TTS](https://coqui.ai/) — Text-to-speech
- [PyAudio](https://people.csail.mit.edu/hubert/pyaudio/) — Audio I/O
- [Silero VAD](https://github.com/snakers4/silero-vad) — Voice activity detection

## Contributing

Contributions, issues, and feature requests are welcome.

## License

MIT License (see LICENSE file if present)

## Contact

Ryan Johnson — [@amdphreak](https://twitter.com/amdphreak)

Project Link: https://github.com/AMDphreak/Desktop-Assistant-AI

Site: https://ryanjohnson.dev

## Security Notes

See `The nature of the security vulnerability.md` for details on a Powershell script parser vulnerability related to speculative execution in batch scripts. This project is designed with security in mind, but always review scripts before running.

## Screenshots

v0.2 - PyQt5 GUI with CoquiTTS.

![screenshot](<v0.2_Screenshot_2025-08-14_235842.png>)

v0.1 - Command line with pyttsx3

![screenshot1](<v0.1_screenshot_20241120_123944.png>)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge
[contributors-url]: https://github.com/AMDphreak/Desktop-Assistant-AI/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge
[forks-url]: https://github.com/AMDphreak/Desktop-Assistant-AI/network/members
[stars-shield]: https://img.shields.io/github/stars/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge
[stars-url]: https://github.com/AMDphreak/Desktop-Assistant-AI/stargazers
[issues-shield]: https://img.shields.io/github/issues/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge
[issues-url]: https://github.com/AMDphreak/Desktop-Assistant-AI/issues
