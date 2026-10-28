<p align="center">
  <img src="assets/icon.png" alt="PortGuard icon" width="128" height="128">
</p>

<h1 align="center">PortGuard</h1>

<p align="center">
  A lightweight macOS menu bar app that monitors your developer ports,<br>
  tracks per-process RAM and CPU usage, and stops forgotten processes with one click.
</p>

<p align="center">
  English | <a href="README.tr.md">Türkçe</a>
</p>

<p align="center">
  <a href="https://github.com/okutaybozkurt/PortGuard/releases">Download</a> &middot;
  <a href="https://github.com/okutaybozkurt/PortGuard">Source code</a> &middot;
  <a href="https://orhankutaybozkurt.com/en/projects/portguard#video">Launch video</a>
</p>

---

## The problem

Development servers (Node, Python, Docker, Go, Flutter) often keep running after a terminal tab is closed. Forgotten ports consume gigabytes of RAM, drain the battery, and cause "address already in use" errors the next time a project starts.

## The solution

PortGuard lives in the macOS menu bar and in a full dashboard window. It shows which process owns which port, how much memory and CPU it uses, and lets you stop the right process safely.

## Features

- **Instant detection:** Lists listening TCP ports and their PIDs within milliseconds.
- **Resource tracking:** Per-process RAM and CPU usage, with daily history and trends.
- **Safe termination:** One-click stop with a confirmation dialog that shows the command and working directory.
- **Port conflict resolver:** Stop and restart the process that holds a busy port.
- **Rule engine:** Threshold-based RAM and CPU rules with notifications or automatic termination.
- **Project scanner:** Reads project files to find the ports a project needs and warns about conflicts.
- **Developer filter:** Hides system services and focuses on development tools.
- **Bilingual:** Turkish and English, switchable at runtime.
- **Native and light:** Built with SwiftUI, with minimal background CPU usage.

## Screenshots

| Developer services | Network activity |
| :---: | :---: |
| ![Developer services](assets/dashboard_dev.png) | ![Network activity](assets/network_activity.png) |
| Only developer tools such as Node, Python and Docker. | Active TCP connections and live bandwidth. |

| History and trends | Rule engine |
| :---: | :---: |
| ![History and trends](assets/dashboard_history.png) | ![Rule engine](assets/portguard_rules.png) |
| Daily RAM peaks, average CPU and port count. | Threshold-based violation detection and actions. |

| Project scanner | Settings |
| :---: | :---: |
| ![Project scanner](assets/portguard_scan_project.png) | ![Settings](assets/settings.png) |
| Port analysis from project files with conflict warnings. | RAM limits, update checks and theme. |

## Requirements

macOS 13.0 or later.

## Links

- Releases and installation: [github.com/okutaybozkurt/PortGuard](https://github.com/okutaybozkurt/PortGuard/releases)
- Launch video: [orhankutaybozkurt.com](https://orhankutaybozkurt.com/en/projects/portguard#video)
- License: MIT

## Author

Developed by [Orhan Kutay Bozkurt](https://github.com/okutaybozkurt) and shared by lokalabs.io.
