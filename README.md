# Linux Sysadmin Anki Deck

![Cards](https://img.shields.io/badge/cards-628-blue)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Format: CrowdAnki](https://img.shields.io/badge/format-CrowdAnki-green)

A 600+ card Anki deck for Linux system administrators, covering practical skills for the **LFCS (Linux Foundation Certified Sysadmin)** exam and everyday Linux work. Built from years of hands-on experience with Debian/Ubuntu, RHEL-family systems, Docker, Kubernetes, and enterprise Linux environments.

---

## How to Import

**Requirements:** [Anki](https://apps.ankiweb.net/) (desktop) + [CrowdAnki add-on](https://ankiweb.net/shared/info/1788670778)

1. Install the CrowdAnki add-on in Anki: `Tools → Add-ons → Get Add-ons → code: 1788670778`
2. Clone or download this repository
3. In Anki: `File → CrowdAnki: Import from disk`
4. Select the `LearningLinux/` folder
5. Click **Import** — the deck appears as **Linux Sysadmin Deck**

> The deck uses two card templates with custom CSS. It is designed for **Anki desktop**; mobile support works but the layout is optimised for larger screens.

---

## Topics Covered

| Topic | Tags |
|-------|------|
| Bash scripting & shell | `BashScripting`, `Scripting` |
| Networking | `Networking`, `DNS`, `DHCP`, `Routing`, `NFS`, `VLan` |
| Security & pen testing | `Security&PenetrationTesting`, `SSH`, `SeLinux`, `Fail2Ban`, `iptables` |
| Firewalls | `Firewalls`, `TCPWrappers`, `iptables` |
| Storage & RAID | `RAID`, `LVM`, `FileSystems`, `Partitions`, `Drives` |
| Package management | `PackageManagement`, `Snapd` |
| Services & init | `Services`, `Booting` |
| Containers | `Docker`, `DockerSwarm`, `Kubernetes`, `GKE`, `GCP` |
| Mail servers | `MailServers`, `Postfix`, `Dovecot`, `Amavis`, `SpamAssassin` |
| Web servers | `WebServers`, `Nginx`, `Apache`, `proFTPd` |
| Databases | `Databases`, `MySQL` |
| Text processing | `AWK`, `Sed`, `Grep`, `Perl` |
| Hardware | `Hardware`, `GPUs`, `Wireless`, `Audio`, `Bluetooth` |
| Monitoring & performance | `Performance`, `Logging`, `KernelRuntimeParameters` |
| Cryptography & certs | `Cryptography`, `Certificates`, `LUKS` |
| Editors & tools | `Vim`, `Nano`, `Git`, `Editors` |
| Multimedia | `Multimedia`, `VideoEditing`, `ImageEditing`, `MusicEditing` |
| LFCS exam prep | `LFCS` |

---

## Card Format

The deck uses two Anki note templates:

- **Code** — Question on the front, shell command on the back, extra Notes field for caveats and context. Ideal for command-line knowledge.
- **Basic-Plus-Media** — Richer layout supporting embedded images and diagrams (used for visual topics such as RAID levels, network architecture, memory management).

Both templates render with custom CSS for a clean, readable look.

---

## Key Tags

| Tag | Meaning |
|-----|---------|
| `Gold` | High-priority card — learn these first |
| `LFCS` | Relevant to the Linux Foundation Certified Sysadmin exam |
| `BestPractice` | Operational best practice or common pitfall |
| `Security&PenetrationTesting` | Security tooling and offensive techniques |
| `GoodHabits` / `BadHabits` | Patterns to adopt or avoid |

---

## Repository Structure

```
.
├── LearningLinux/
│   ├── deck.json       # CrowdAnki deck (all cards + configuration)
│   └── media/          # Embedded images and CSS
├── scripts/
│   └── clean_deck.py   # Cleanup script (removes off-topic cards, fixes typos)
├── CONTRIBUTING.md
├── LICENSE
└── README.md
```

---

## Contributing

Corrections and improvements are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## License

[MIT](LICENSE) © Carlo Martini

Cards that include screenshots from the Linux Foundation course materials (LFS01) are used for educational purposes and remain subject to the original copyright.
