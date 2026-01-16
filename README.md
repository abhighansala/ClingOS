# 🖥️ ClingOS  
<p align="center">
  <img src="assets/logo.png" alt="Cling logo" width="200">
</p>

<h1 align="center">Cling</h1>
**A next-generation Linux desktop OS built in Rust — fast, fluid, cloud-connected.**

ClingOS aims to deliver a polished, fluid, modern desktop experience powered by **Linux + Rust**, built around the **COSMIC compositor** with a **completely new shell** called **Cling Shell**.  

Inspired by UX quality on macOS and the freedom of Linux, ClingOS will eventually support desktop ↔ mobile continuity using a future AOSP-based phone OS.

---

## 🔥 Vision

ClingOS is not a theme.  
It is a **new desktop environment from scratch**, prioritizing:

- ⚡ Speed + memory efficiency using Rust
- 🖥 Wayland-native compositor animations
- 🎨 Beautiful UI/UX with glass, blur & fluid transitions
- 🧩 Modular apps & system components
- ☁ Future ClingCloud sync for cross-device continuity
- 📱 Planned AOSP mobile integration

> The goal is a smooth, elegant desktop — functional like Linux, polished like macOS.

---

## 📦 Project Structure

```
ClingOS/
├── core/                        # System backend
│   ├── cling-comp               # Wayland compositor in Rust
│   ├── cling-session
│   ├── cling-settings-daemon
│   ├── cling-notifications
│   ├── cling-randr
│   ├── cling-osd
│   ├── cling-idle
│   ├── cling-applibrary
│   ├── cling-workspaces-epoch
│   ├── cling-bg
│   └── xdg-desktop-portal-cling
│
├── shell/                        # New UI shell layer (main dev focus)
│   └── cling-shell/              # Rust + Iced desktop shell
│       ├── src/
│       └── assets/
│
├── apps/                         # System apps (future)
│   ├── cling-files/              # File Manager
│   ├── cling-settings-ui/        # Settings frontend
│   ├── cling-store/              # App Store
│   └── ...
│
├── services/                     # Cloud sync daemons (future)
│   ├── cling-syncd/
│   ├── cling-handsoffd/
│   └── cling-clipboardd/
│
└── iso/                          # Image builder (future release)
    └── build-image.sh
```


---

## 🧱 Tech Stack

| Layer | Technology |
|---|---|
| Kernel | Linux |
| Compositor | `cling-comp` (Rust + Smithay) |
| Shell UI | `cling-shell` (Rust + Iced) |
| Packaging | Flatpak + custom `.clingpkg` (future) |
| Cloud Sync | Rust + Supabase backend (future) |
| Mobile | AOSP-based ClingOS Mobile (future) |

---

## 🚧 Development Status

| Feature | Status |
|---|---|
| Repository Base | ✔ Started |
| Cling Shell | ⏳ In Development |
| Top Bar | ⏳ Planned |
| Dock | ⏳ Planned |
| App Launcher | ⏳ Planned |
| Mission Control | ⏳ Planned |
| Notification Center | ⏳ Planned |
| ClingCloud Sync | ❗ Future milestone |
| Installer ISO | ❗ Future |

> This project is currently **pre-alpha** — not usable as a desktop environment yet.

---

## Roadmap

| Stage | Goal |
|---|---|
| 0.1 | Cling Shell creates a window |
| 0.2 | Top Bar UI |
| 0.3 | Dock with pinned apps |
| 0.4 | Spotlight-like Launcher (Applibrary) |
| 0.6 | Workspace overview (Mission Control) |
| 0.8 | Notification + Control Center |
| 1.0 | First daily-driver alpha |
| 2.0 | ClingCloud sync + AOSP integration |

---

## Contributing

Contributions are welcome as development moves forward.

We will need:

- Rust developers (Shell, compositor, protocol integration)
- UI/UX designers
- Package maintainers
- Cloud backend devs (Rust + Supabase)
- Documentation helpers

Until shell fundamentals are stable, PRs may be limited.

---

## Disclaimer

ClingOS is **not affiliated with Pop!\_OS or System76**.  
COSMIC components remain under their original licenses.  
UI layers will be replaced to avoid trademark conflict.

---

### 🌟 ClingOS — Clean. Fluid. Rust At The Core.
