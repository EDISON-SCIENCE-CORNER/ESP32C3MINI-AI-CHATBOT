<div align="center">

# 🤖 ESP32-C3 Mini AI Chatbot

### A pocket-sized voice AI assistant – talk to it, and it talks back!

[![YouTube](https://img.shields.io/badge/YouTube-Edison%20Science%20Corner-red?style=for-the-badge&logo=youtube)](https://www.youtube.com/@EDISON_SCIENCE_CORNER)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Support-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black)](https://buymeacoffee.com/esclabs)
[![Flash Firmware](https://img.shields.io/badge/Flash%20Firmware-ESC%20Labs-blue?style=for-the-badge&logo=espressif&logoColor=white)](https://www.esclabs.in/esclab-flasher/)

</div>

---

## ✨ Features

- 🎙️ **Voice input** – I²S digital microphone captures your voice
- 🧠 **AI-powered replies** – ask questions and chat over Wi-Fi
- 🔊 **Voice output** – answers spoken through the I²S amplifier and speaker
- 🖥️ **OLED display** – shows status and responses
- 🔋 **Battery powered** – rechargeable Li-Po with USB charging
- 🖨️ **3D-printed case** – compact, portable design
- ⚡ **No coding needed** – flash the firmware straight from your browser

---

## 🧰 Components Required

| Component | Details |
|---|---|
| Microcontroller | ESP32-C3 Super Mini |
| Display | 0.96" / 1.3" I²C OLED |
| Microphone | INMP441 I²S MEMS microphone |
| Amplifier | MAX98357A I²S amplifier |
| Speaker | Small 4–8 Ω speaker |
| Charger | TP4056 Li-Po charging module |
| Battery | 3.7V Li-Po (110 mAh used in the build) |
| Enclosure | 3D-printed – `3D FILE/3D FILE C3MINI AI.stl` |
| Misc | Wires, switch (optional), soldering kit |

---

## 🔌 Wiring

📐 Full circuit: **`circuit diagram.jpg`**

### OLED Display
| OLED | ESP32-C3 |
|---|---|
| SDA | GPIO 21 |
| SCL | GPIO 20 |
| VCC | 3.3V / 5V |
| GND | GND |

### INMP441 Microphone
| Microphone | ESP32-C3 |
|---|---|
| SCK / BCLK | GPIO 2 |
| WS / LRCK | GPIO 1 |
| SD / DOUT | GPIO 8 |
| L/R | GND |
| VDD | 3.3V |
| GND | GND |

### MAX98357A Amplifier
| MAX98357A | ESP32-C3 |
|---|---|
| BCLK | GPIO 2 |
| LRC / LRCK | GPIO 1 |
| DIN | GPIO 3 |
| VIN | 5V |
| GND | GND |

> 💡 The microphone and amplifier share the **BCLK (GPIO 2)** and **LRCK (GPIO 1)** lines.

### Power
| TP4056 | Connection |
|---|---|
| B+ / B− | Li-Po battery + / − |
| OUT+ | ESP32-C3 5V |
| OUT− | ESP32-C3 GND |

---

## ⚡ Flash the Firmware

No Arduino IDE needed – flash directly from your browser:

👉 **[ESC Labs Web Flasher](https://www.esclabs.in/esclab-flasher/)**

1. Open the flasher in **Google Chrome** or **Microsoft Edge** on a computer
2. Connect the ESP32-C3 Super Mini with a USB **data** cable
3. Select the **AI Chatbot** firmware
4. Click **Connect**, choose your board's COM port
5. Click **Flash** and wait for it to finish ✅

> 🛠️ **Board not detected?** Hold the **BOOT** button, press and release **RESET**, then release **BOOT** and try connecting again.

---

## 🖨️ 3D-Printed Case

- File: **`3D FILE/3D FILE C3MINI AI.stl`**
- Recommended layer height: **0.2 mm**
- Material: PLA

---

## 📁 Repository Files

| File | Description |
|---|---|
| `circuit diagram.jpg` | Complete wiring diagram |
| `3D FILE/3D FILE C3MINI AI.stl` | 3D-printable enclosure |

---

## 🎥 Watch the Build

Full build video and more projects on my YouTube channel:

👉 **[Edison Science Corner](https://www.youtube.com/@EDISON_SCIENCE_CORNER)**

Don't forget to **Like, Share & Subscribe!** 🔔

---

## ☕ Support

If you enjoyed this project and want to support more builds:

<a href="https://buymeacoffee.com/esclabs" target="_blank">
  <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="50">
</a>

---

## ⭐ Show Your Love

If you like this project, give the repo a **star ⭐** and share your builds!

<div align="center">

Made with ❤️ by **[Edison Science Corner](https://www.youtube.com/@EDISON_SCIENCE_CORNER)** · **[ESC Labs](https://www.esclabs.in)**

</div>
