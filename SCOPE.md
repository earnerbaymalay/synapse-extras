# Synapse Extras — Scope & Architecture Specification

> **Repository:** `earnerbaymalay/synapse-extras`  
> **Parent Ecosystem:** SynapseOS  
> **Distribution Model:** Opt-In / Modular Packages  

---

## 1. Vision & Purpose
SynapseOS core is strictly scoped to high-throughput agentic computing, zero telemetry, and kernel performance. To prevent base image bloat, **Synapse Extras** houses all community, aesthetic, and domain-specialized add-ons that users can opt into during Calamares installation (via the Netinstall screen) or post-install via `synapse extras install <pack>`.

---

## 2. Component Pillars

### A. Extended Aesthetics & Cyberdeck Themes (`themes/`)
- Additional metallic wallpaper suites (Smoked Obsidian, Crimson Tower, Sapphire Monolith).
- Extended terminal colorways (Catppuccin Macchiato, Tokyo Night Cyber, OLED Pure Black).
- Alternative Plymouth boot sequences and GRUB high-DPI splash assets.

### B. Cyberdeck Audio Synthesis (`audio/`)
- Bespoke mechanical chime soundfonts for boot, terminal notifications, and SDDM greeter focus.
- Low-latency PipeWire / WirePlumber audio profiles for external DACs and professional monitoring.

### C. Advanced Agent Workflow Packs (`workflows/`)
- Scoped RF Penetration Testing Automation (WiFi beacon surveys, token harvesters, automated PCAP auditors).
- Offline Documentation Synthesizers (local ArchWiki, Rust docs, and Linux manpages indexed into `synapse mem`).
- Custom Function Packs for `SynapseCli` (`syn-fn`).

---

## 3. Packaging & Installation Matrix
- **Arch Linux PKGBUILDs**: Packaged as modular split packages:
  - `synapse-extras-themes`
  - `synapse-extras-audio`
  - `synapse-extras-workflows`
  - `synapse-extras-all` (meta-package)
- **Calamares Netinstall Integration**: Integrated as optional checkboxes in `netinstall.yaml`.
