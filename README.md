<a id="readme-top"></a>
<div align="center">
  <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/graphs/contributors"><img src="https://img.shields.io/github/contributors/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge" alt="Contributors"></a>
  <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/network/members"><img src="https://img.shields.io/github/forks/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge" alt="Forks"></a>
  <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/stargazers"><img src="https://img.shields.io/github/stars/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge" alt="Stargazers"></a>
  <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/issues"><img src="https://img.shields.io/github/issues/AMDphreak/Desktop-Assistant-AI.svg?style=for-the-badge" alt="Issues"></a>

  <h3 align="center">Desktop Assistant AI</h3>
  <p align="center">
    An AI to help users when they don't know what to do, with emphasis on code help.
    <br />
    <br />
    <a href="https://desktop-tooling.github.io/docs/desktop-assistant-ai/"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/issues">Report Bug</a>
    &middot;
    <a href="https://github.com/AMDphreak/Desktop-Assistant-AI/issues">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#security-notes">Security Notes</a></li>
    <li><a href="#screenshots">Screenshots</a></li>
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

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* **GUI** — [![PyQt5][PyQt.badge]][PyQt-url]
* **AI / speech**
  * [![OpenAI][OpenAI.com]][OpenAI-url] — ChatGPT and Whisper
  * [Coqui TTS](https://coqui.ai/)
  * [Silero VAD](https://github.com/snakers4/silero-vad)
* **Audio** — [PyAudio](https://people.csail.mit.edu/hubert/pyaudio/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

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

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

After installation, launch the assistant using `run.ps1`. The app will show a loading screen while the Whisper and Coqui TTS models load, then present the main window for interaction.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

Contributions, issues, and feature requests are welcome.

### Top contributors

<a href="https://github.com/AMDphreak/Desktop-Assistant-AI/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=AMDphreak/Desktop-Assistant-AI" alt="contributors" />
</a>

For per-person profile links, prefer [all-contributors](https://allcontributors.org/).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for the project history.

## License

MIT License (see LICENSE file if present)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

Ryan Johnson — [@amdphreak](https://twitter.com/amdphreak)

Project Link: [https://github.com/AMDphreak/Desktop-Assistant-AI](https://github.com/AMDphreak/Desktop-Assistant-AI)

Site: [https://ryanjohnson.dev](https://ryanjohnson.dev)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Security Notes

See `The nature of the security vulnerability.md` for details on a Powershell script parser vulnerability related to speculative execution in batch scripts. This project is designed with security in mind, but always review scripts before running.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Screenshots

v0.2 - PyQt5 GUI with CoquiTTS.

![screenshot](<v0.2_Screenshot_2025-08-14_235842.png>)

v0.1 - Command line with pyttsx3

![screenshot1](<v0.1_screenshot_20241120_123944.png>)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[PyQt.badge]: https://img.shields.io/badge/PyQt5-41CD52?style=for-the-badge&logo=qt&logoColor=white
[PyQt-url]: https://riverbankcomputing.com/software/pyqt/intro
[OpenAI.com]: https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white
[OpenAI-url]: https://openai.com/
