# Ubuntainium

[![GitHub stars](https://img.shields.io/github/stars/sm00thbrains/Ubuntainium)](https://github.com/sm00thbrains/Ubuntainium/stars)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Obtainium for Ubuntu** — Update GitHub apps *outside* of `apt`. No PPAs. No stale repos. No 8-year-old packages haunting your system.

Tired of Ubuntu's repos lagging years behind? Ubuntainium watches GitHub releases and auto-updates your tools. `.deb`, `.AppImage`, binaries — all handled.

```bash
curl -fsSL get.ubuntainium.sh | bash
ubuntainium add windterm kingToolbox/WindTerm deb "WindTerm_.*amd64\\.deb" \
  "sudo dpkg -i {{file}} || sudo apt install -f -y"
ubuntainium  # Updates everything
