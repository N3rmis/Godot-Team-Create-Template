# Godot Team Create — Project Template

A starter project template for **Godot 4** with the **Team Create** real-time collaborative editing plugin pre-installed and pre-enabled.

Create games, prototypes, and levels together with your friends and teammates in real time for the Godot Engine!

---

## Features

- **Live Scene Synchronization**: Real-time multi-user editing for nodes, transforms, properties, animations, and in-memory sub-resources (materials, primitive meshes, shapes).
- **Collaborative Code Editing**: Live script editing with 100ms debounced line diffs, live colored presence carets, collaborator name badges, and selection highlighting on `CodeEdit`.
- **Single-Port Architecture**: Handles both UDP multiplayer RPCs and high-throughput TCP HTTP binary asset streaming over a single port (`25567` by default).
- **One-Click Host LAN**: Host directly from the Godot editor or spin up a dedicated headless background server with a single click.
- **In-Editor Team Chat**: Integrated bottom-panel team messaging with BBCode formatting, custom username colors, and image attachment sharing.
- **Distributed Node Locking**: Prevents editing collisions and gizmo jitter by locking selected nodes during active manipulation.
- **Headless Server & VPS Deployment**: Includes automated export tools for running dedicated 24/7 synchronization servers on Linux VPS or Windows.

---

## Quick Start

1. **Open the Project**:
   - Open this project in **Godot 4.2+** (compatible with Godot 4.2, 4.3, and 4.7+).
   - The **Team Create** plugin is enabled automatically.
2. **Find the Dock**:
   - Look at the top-left editor dock: find the **Team Create** tab.
3. **Host or Join**:
   - **To Host**: Enter your username and click **Host LAN**. (Or click **Host** to use an existing server).
   - **To Join**: Enter your teammate's IP (e.g. `192.168.1.50:25567` or public IP / VPS domain) and click **Join**.
4. **Start Building Together**:
   - Move nodes, tweak properties in the Inspector, edit scripts in the Script Editor, or chat in the **Team Chat** panel at the bottom!

---

## Network & Port Forwarding

- **Default Port**: `25567` (UDP Multiplayer & TCP HTTP Asset Streaming).
- If hosting over the internet (outside your local Wi-Fi / LAN), ensure port `25567` (both **UDP** and **TCP**) is forwarded on your router to your host PC, or run a dedicated headless server on a VPS.
- You can change the port at any time via the `/port <number>` server command or the `/filetimeout <seconds>` command for adjusting HTTP asset transfer timeouts.

---

## Automatic Upstream Synchronization

This template repository is automatically synchronized with the upstream plugin repository:
👉 [https://github.com/N3rmis/Godot-Team-Create](https://github.com/N3rmis/Godot-Team-Create)

Any updates, bug fixes, and new features pushed to the main plugin repository are automatically merged into this project template via GitHub Actions.

---

## 📄 License

This template and the Team Create plugin are released under the [MIT License](LICENSE).
Created by **N3rmis** (2026).
