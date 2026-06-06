# ◢ NETBREAKER ◣
### Terminal Hacking Simulation Game

A browser-based, terminal-aesthetic hacking game where players solve real computer science puzzles to progress through missions. No backend required — runs entirely in the browser.

---

## Play It
Open `index.html` in any browser. No install, no dependencies.

**Live via GitHub Pages:** `https://<your-username>.github.io/netbreaker`

---

## Choose Your Path

| Path | Role | Playstyle |
|------|------|-----------|
| **GHOST** | Black Hat | Breach systems, crack passwords, cover tracks |
| **SENTINEL** | Ethical Hacker | Detect intrusions, patch vulnerabilities, defend |

Both paths share the same puzzle engine but with different objectives and framing per puzzle.

---

## Missions & Puzzles

| Mission | Name | Puzzles |
|---------|------|---------|
| M01 | Cold Boot | Decode Message, File Investigation |
| M02 | Deep Trace | Log Analysis, Network Mapping |
| M03 | Root Access | Password Cracking, Process Investigation, Permissions |
| M04 | Ghost Protocol | Binary Decode, Digital Breadcrumbs |
| M05 | Zero Day | Timed Breach |

### Puzzle Types
- **File Investigation** — navigate a fake filesystem, find hidden files
- **Log Analysis** — read server logs, identify attackers or erase your tracks
- **Password Cracking** — crack MD5 hashes using common patterns
- **Decode Messages** — Base64, hex, binary, Caesar cipher
- **Network Mapping** — identify open ports and unauthorized hosts
- **Digital Breadcrumbs** — follow a chain of clues across DNS, logs, and configs
- **Process Investigation** — find malicious or anomalous PIDs
- **Permissions Puzzle** — exploit or lock down misconfigured Unix permissions
- **Binary Decode** — convert 8-bit binary groups to ASCII
- **Timed Puzzles** — solve under a countdown timer

---

## Terminal Commands

```
missions              List all missions
start <id>            Begin a mission (e.g. start M01)
ls / ls -la           List directory contents
cat <file>            Read a file
grep <pattern> <file> Search a file
decode --base64 <str> Decode a Base64 string
decode --hex <str>    Decode a hex string
crack --hash <hash>   Attempt to crack a hash
ping <ip>             Ping an IP address
ps aux                List running processes
chmod <perms> <file>  Change permissions
whoami / uptime       System info
clear                 Clear terminal
help / man            Open Operator's Manual
↑ / ↓                 Navigate command history
```

---

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `netbreaker`)
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages**
4. Set source to `main` branch, root folder
5. Your game is live at `https://<username>.github.io/netbreaker`

---

## Roadmap

- [ ] More missions (10+ planned)
- [ ] More puzzle types (steganography, routing, corrupted data recovery, SQL injection)
- [ ] Story narrative between missions (intercepted emails, news feeds)
- [ ] Navigable fake filesystem (`cd`, `cat` on mission files)
- [ ] Sound effects (keyclick, alert beeps)
- [ ] Save/load progress via localStorage
- [ ] Multiplayer PvP mode (Ghost vs Sentinel) via Firebase

---

## Tech Stack

| Layer | Tech |
|-------|------|
| Game logic | Vanilla JavaScript |
| UI | HTML + CSS (no frameworks) |
| Fonts | Google Fonts (Share Tech Mono, VT323) |
| Hosting | GitHub Pages |
| Future multiplayer | Firebase Realtime Database |

Single file. Zero dependencies. Zero build step.

---

*Built with Claude — expand, modify, and make it your own.*
