<div align="center">

# ☁️ ServerSim Cloud

**A browser-based cloud hosting, data center, and server operating system simulator.**

Explore a fictional infrastructure lab inspired by cloud provider dashboards and game-server control panels — right in your browser.

[Features](#-features) · [Getting Started](#-getting-started) · [Project Status](#-project-status) · [License](#-license)

</div>

---

> [!IMPORTANT]
> **This is an educational simulation, not a real hosting provider.** It does not create cloud instances, run actual Linux commands, open ports, host databases, or start Minecraft servers. Metrics, IP addresses, service states, and player counts are demo data.

## ✨ Features

- **Cloud dashboard** — view fictional compute instances, activity events, and resource utilization.
- **Virtual server management** — create, start, stop, restart, and remove simulated instances with configurable CPU, RAM, region, and role.
- **Data center explorer** — inspect illustrative racks, compute nodes, storage, switches, power, and cooling.
- **Simulated Linux terminal** — try safe, predefined examples such as `help`, `ls`, `top`, `free -h`, `df -h`, `ip addr`, `docker ps`, and service-status commands.
- **Server OS desktop** — use mock shortcuts for system monitoring, storage, networking, containers, and web services.
- **Web hosting panel** — add fictional static sites, Node apps, and reverse proxies.
- **Database hosting panel** — create demo PostgreSQL, MongoDB, and Redis entries.
- **Game hosting panel** — create mock Minecraft Java, Minecraft Bedrock, and generic game-server entries.
- **Network panel** — explore private IP addresses and example firewall rules.
- **Local persistence** — save demo state in your browser using `localStorage`.
- **JSON export** — download your current demo environment.
- **Responsive UI** — designed for desktop and mobile screens.
- **No build step** — the front end is a standalone HTML page.

## 🖥️ Getting Started

### Run locally

1. Clone or download this repository.
2. Open `index.html` in a modern browser.

Or serve the folder locally with Python:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

### Deploy to GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Under the build and deployment settings, select **Deploy from a branch**.
3. Choose the `main` branch and the `/ (root)` folder.
4. Save and wait for the deployment to finish.

You can also deploy it as a static site on a compatible hosting service. No backend or environment variables are required for the current demo.

## 🧭 Project Sections

| Section | What it demonstrates |
| --- | --- |
| Overview | Instance totals, resource charts, and recent events |
| Virtual servers | Simulated instance lifecycle and configuration |
| Data center | Rack layouts and fictional facility metrics |
| Terminal | A fixed set of simulated Linux-like commands |
| Server OS | Mock desktop shortcuts and system utilities |
| Web hosting | Example website and application service entries |
| Databases | Fictional database service entries |
| Game hosting | Mock game instances and player counts |
| Network | Example private addresses and firewall policies |
| Settings | Local preferences, reset, and data cleanup |

## 💾 Local Demo Data

The simulator stores its demo instances, events, service entries, and network rules in your browser's `localStorage`. This data stays in that browser profile and is not synchronized to a server.

- Use **Reset demo** to restore the initial sample environment.
- Use **Settings → Clear local demo data** to remove saved demo state.
- Use **Export data** to download a JSON snapshot.

Avoid entering passwords, API keys, tokens, or other secrets. The project does not need them.

## 🛠️ Technology

- HTML
- CSS
- Vanilla JavaScript
- Browser `localStorage`

The current implementation keeps the app in `index.html` to make it easy to inspect, modify, and host. It does not currently integrate with AWS, Pterodactyl, Docker, real Linux virtual machines, database engines, or game-server providers.

## 🗺️ Project Status

ServerSim Cloud is an early-stage interface and infrastructure simulation. The current goal is to provide a polished playground for learning about hosting concepts before considering any real integrations.

Possible future directions include:
- Separating the single-page app into maintainable HTML, CSS, and JavaScript files.
- Adding more detailed service logs and instance configuration.
- Improving accessibility and localization.
- Adding optional integrations only when a real backend and appropriate security controls exist.

These are ideas, not promises or implemented features.

## 🤝 Contributing

Suggestions, bug reports, and pull requests are welcome. When contributing:

1. Keep demo actions clearly labelled as simulations.
2. Do not imply that a simulated action creates real infrastructure.
3. Never collect or expose user secrets.
4. Describe manual testing performed in pull requests.

## 📄 License

This project is released under the **MIT License**. See [LICENSE](LICENSE) for details.

---

<div align="center">

Made for experimenting with cloud and server concepts — without needing a server bill.

</div>
