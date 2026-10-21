# TheKikGen.github.io

Welcome to the official web utilities portal of **TheKikGen Labs**. This repository hosts a collection of pure client-side, browser-based tools leveraging modern Web APIs like **Web MIDI**, **WebHID**, and **Web Serial** to interface, configure, and debug DIY hardware music projects, MIDI gear, and advanced sequencers.

---

### 🎛️ MPC Standalone Utilities (Akai MPC & Force Ecosystem)

*   **[INMUSIC AZ01 CONTAINER SUITE](https://TheKikGen.github.io/MPC/inmusic_az01_container_suite.html)** – An advanced, memory-safe firmware image analyzer and workspace utility. It features a standalone, browser-based user interface using a pseudo-mount layout and embedded C-WASM XZ decompression to let you audit and extract update packages directly from your browser (see all projects at https://github.com/TheKikGen/MPC-LiveXplore).
    *   **Firmware Analyzer:** Instantly slices and parses the first 64 KB header and EOF trailers of official or custom `.img` / `.bin` containers safely, without overloading system RAM even with multi-gigabyte files.
    *   **RootFS Explorer & Hex Inspector:** Provides built-in visual inspection components to navigate inner file systems and analyze raw hex streams of payload binaries.
    *   **Container Builder & Exporters:** Houses front-end controllers to configure new firmware images alongside native Python/Bash CLI standalone exporters.

### 🎵 USBMIDIKLIK eco system (project at https://github.com/TheKikGen/USBMidiKliK4x4)

*   **[umk4x4-Configurator.html](https://TheKikGen.github.io/umk4x4-Configurator.html**
The dedicated graphical configuration interface for the **[USBMidiKliK4x4 (UMK4x4)](https://github.com/TheKikGen/USBMidiKliK4x4)** project (the multi-port USB MIDI interface for STM32F103/Bluepill boards). It allows you to visually configure complex MIDI routing tables, filters, pipes, and standalone behaviors over MIDI SysEx.

*   **[MidiSysExUtility.html](https://TheKikGen.github.io/MidiSysExUtility.html)**
A lightweight standalone web utility designed to send, receive, and analyze **MIDI System Exclusive (SysEx)** messages. Ideal for backing up firmware dumps, restoring presets, or debugging custom SysEx implementations on synthesizers and controllers.

*   **[tkg-hid-webcli.html](https://TheKikGen.github.io/tkg-hid-webcli.html)**
A browser-based Human Interface Device (HID) command-line interface helper. It utilizes the native **WebHID API** to talk directly to the TKG HID bootloader (https://github.com/TheKikGen/stm32-tkg-hid-bootloader) for low-level configuration and devices firmware updates without requiring native desktop software.

*   **[SerialTerm.html](https://TheKikGen.github.io/SerialTerm.html)**
A simple, portable **Web Serial terminal** running entirely in your browser. Connect directly to microcontrollers (STM32, Arduino, ESP32) via USB-to-UART bridges or native CDC serial ports at standard baud rates (e.g., 115200) to view debug logs or interactive menus.

*   **[webmidi.html](https://TheKikGen.github.io/webmidi.html)**
A diagnostic monitoring tool leveraging the **Web MIDI API** to discover hardware MIDI input/output ports connected to your system, test low-level message flows, and log raw MIDI streams in real time.

---

## 🚀 Key Features

* **Zero Installation:** Every tool runs 100% locally in your web browser. No external drivers, Node.js setups, or desktop installations required.
* **Privacy Focused:** Your data, configuration dumps, and MIDI streams never leave your machine—no remote server interactions.
* **Hardware Friendly:** Tailored explicitly to complement other open-source projects hosted under [TheKikGen GitHub profile](https://github.com) (such as *USBMidiKliK*, *MPC-LiveXplore*, and custom STM32 utilities).

## 📋 Requirements & Browser Support

To interact with physical hardware devices, these tools require native access to hardware communication stacks. It is highly recommended to use modern **Chromium-based browsers** (e.g., **Google Chrome**, **Microsoft Edge**, or **Opera**) which fully implement:
* Web MIDI API (including SysEx exclusive access privileges)
* WebHID API
* Web Serial API

*Note: Safari and Firefox do not currently support WebHID or Web Serial APIs natively.*

---

## 🤝 Related Main Projects

Check out the core hardware firmware and hacks that these web tools interact with:
* 🎚️ **[USBMidiKliK4x4](https://github.com)** - Multi-port USB MIDI interface for STM32F103.
* 🤖 **[MPC-LiveXplore](https://github.com/MPC-LiveXplore)** - Custom standalone software hacks, mods, toolkit, and tools for the Akai MPC & Force ecosystem.

---

## 📄 License & Issues

This repository and its web-facing tools are maintained by **TheKikGen Labs**. Feel free to explore the source code directly or open an issue on the tracker if you encounter any bugs.
