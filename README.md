# Modbus RTU Address Scanner

A lightweight Windows tool for scanning **Modbus RTU devices** on an RS-485 bus.  
This application lets you quickly find which slave addresses respond, read test registers, and verify communication settings.

---

## 🚀 Quick Start

1. Go to the [Releases](../../releases) page.
2. Download the latest **`Modbus RTU Address Scanner.exe`**.
3. Run it – **no Python installation required**.
4. Select:
   - **COM port** of your USB–RS485 adapter  
   - **Baud rate** (e.g. 9600)  
   - **Parity / Stop bits** (usually N,1)  
   - **Timeout** (e.g. 0.3 s)  
5. Choose an address range (e.g. 1–247) and a test register (try 0, 1, or 100).  
6. Click **Scan** – responding devices will appear in the results table.

---

## ✨ Features
- Scan any Modbus RTU address range (0–247).
- Select COM port, baud rate, parity, stop bits, and timeout.
- Read holding register values from a configurable test register.
- Detect alive units even if registers return an exception.
- Live log output for troubleshooting.
- Standalone `.exe` – no dependencies or installation needed.

---

## 🧾 Notes
- Many devices use register **1** for temperature or status.  
- If nothing appears:
  - Try test registers `0`, `1`, or `100`.
  - Swap A/B lines on RS-485.
  - Increase timeout to `0.5 s`.
  - Check that no other Modbus master is connected at the same time.

---

## 📜 License
This project is licensed under the [MIT License](LICENSE).  
You are free to use, copy, and distribute the software for personal or commercial purposes, with attribution.

---
