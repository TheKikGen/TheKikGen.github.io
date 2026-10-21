# TheKikGen.github.io

Welcome to the official web utilities portal of **TheKikGen Labs**. This repository hosts a collection of pure client-side, browser-based tools leveraging modern Web APIs like **Web MIDI** and **WebHID** to interface, configure, and debug DIY hardware music projects, MIDI gear, and advanced sequencers.

🌐 **Live Access:** [https://github.io](https://github.io)

---

## 🛠️ Available Web Tools & Utilities

### 🎛️ [umk4x4-Configurator.html](https://github.io/umk4x4-Configurator.html)
The dedicated graphical configuration interface for the **[USBMidiKliK4x4 (UMK4x4)](https://github.com/TheKikGen/USBMidiKliK4x4)** project (the multi-port USB MIDI interface for STM32F103/Bluepill boards). It allows you to visually configure complex MIDI routing tables, filters, pipes, and standalone behaviors over MIDI SysEx.

### 📝 [MidiSysExUtility.html](https://github.io/MidiSysExUtility.html)
A lightweight standalone web utility designed to send, receive, and analyze **MIDI System Exclusive (SysEx)** messages. Ideal for backing up firmware dumps, restoring presets, or debugging custom SysEx implementations on synthesizers and controllers.

### 🔌 [tkg-hid-webcli.html](https://github.io/tkg-hid-webcli.html)
A browser-based Human Interface Device (HID) command-line interface helper. It utilizes the native **WebHID API** to talk directly to compatible USB HID bootloaders and hardware (such as the `stm32-tkg-hid-bootloader`) for low-level configuration and firmware updates without requiring native desktop software.

### 💻 [SerialTerm.html](https://github.io/SerialTerm.html)
A simple, portable **Web Serial terminal** running entirely in your browser. Connect directly to microcontrollers (STM32, Arduino, ESP32) via USB-to-UART bridges or native CDC serial ports at standard baud rates (e.g., 115200) to view debug logs or interactive menus.

### 🎵 [webmidi.html](https://github.io/webmidi.html)
A diagnostic monitoring tool leveraging the **Web MIDI API** to discover hardware MIDI input/output ports connected to your system, test low-level message flows, and log raw MIDI streams in real time.

---

## 🚀 Key Features

* **Zero Installation:** Every tool runs 100% locally in your web browser. No external drivers, Node.js setups, or software installs required.
* **Privacy Focused:** Your data, configuration dumps, and MIDI streams never leave your machine—no remote server interactions.
* **Hardware Friendly:** Tailored explicitly to complement other open-source projects hosted under [TheKikGen GitHub profile](https://github.com/TheKikGen) (such as *USBMidiKliK*, *MPC-LiveXplore*, and custom STM32 utilities).

## 📋 Requirements & Browser Support

To interact with physical hardware devices, these tools require native access to hardware communication stacks. It is highly recommended to use modern **Chromium-based browsers** (e.g., **Google Chrome**, **Microsoft Edge**, or **Opera**) which fully implement:
* Web MIDI API (including SysEx exclusive access privileges)
* WebHID API
* Web Serial API

*Note: Safari and Firefox do not currently support WebHID or Web Serial APIs natively.*

---

## 🤝 Related Projects

Check out the core hardware firmware and hacks that these web tools interact with:
* 🎚️ **[USBMidiKliK4x4](https://github.com/TheKikGen/USBMidiKliK4x4)** - Multi-port USB MIDI interface for STM32F103.
* 🤖 **[MPC-LiveXplore](https://github.com/TheKikGen/MPC-LiveXplore)** - Custom standalone software hacks, mods, and embedded tools for the Akai MPC & Force ecosystem.

---

## 📄 License

This repository and its web-facing tools are maintained by **TheKikGen Labs**. Feel free to explore the source code directly or open an issue on the tracker if you encounter any bugs.
