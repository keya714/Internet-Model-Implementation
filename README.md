# 🌐 Internet Model Simulation in C++ (TCP/IP Layers Visualizer)

This project is a **graphical simulation** of the **Internet (TCP/IP) layered communication model**, implemented in **C++** using the **graphics.h** library. It visually demonstrates how data flows from sender to receiver across the five networking layers: **Application**, **Transport**, **Network**, **Data Link**, and **Physical**.

---

## 🎯 Key Features

- 📡 **Layer-by-layer packet visualization**
- 💻 **LAN-to-LAN communication simulation via Router**
- 🔁 **Two-way communication (sender ↔ receiver)**
- 📄 **MAC & IP address headers displayed**
- 🎨 **Fully animated with real-time mouse interaction**
- 🖱️ **Graphical interaction via mouse clicks on sender/receiver nodes**

---

## 🛠️ Technologies Used

| Component           | Details                        |
|--------------------|---------------------------------|
| Language           | C++                             |
| Graphics Library   | `graphics.h` (Borland/WinBGI)   |
| Platform           | Windows                         |
| Interface          | GUI Simulation (2D animation)   |
| Dependencies       | WinBGI, Windows API, `<conio.h>`|

---

## 📐 Layers Simulated

1. **Application Layer** – Message generation ("HELLO!")
2. **Transport Layer** – Header addition (H1)
3. **Network Layer** – IP routing logic (`10-11`, `71-73`, etc.)
4. **Data Link Layer** – MAC addressing (e.g., `AA-RT`, `OP-QZ`)
5. **Physical Layer** – Binary representation (e.g., `1 0 0 1`)

---

## 🖥️ How It Works

- On launch, a **network topology** with two LANs and a router is displayed.
- Click on any **sender node** in LAN1 and any **receiver node** in LAN2.
- The program then:
  1. Draws the path data would take through all 5 layers.
  2. Adds layer-specific headers at each stage.
  3. Shows routing via the router (if across networks).
  4. Displays a final "HELLO" message at the receiver.

---

## 📸 Visual Components

- 💻 PCs for sender and receiver
- 🔄 Router connecting the LANs
- ↔️ Arrows representing data transmission
- 🧱 Boxes for each layer with color-coded labels

---

## 🏁 How to Run

1. **Install a C++ compiler** with graphics support like WinBGI or Turbo C++ on Windows.
2. **Place required image files** (e.g., `2.jpg`, `3.jpg`) in correct paths or modify the `readimagefile()` paths in code.
3. **Compile the program**:

    ```bash
    g++ Internet\ Model.cpp -lbgi -lgdi32 -lcomdlg32 -luuid -loleaut32 -lole32 -o internet_model
    ```

4. **Run the executable**:

    ```bash
    ./internet_model
    ```

---

## 🎮 Controls

- 🖱️ Click on a **sender node** (LAN1) and then a **receiver node** (LAN2).
- 🔁 Use arrow keys to navigate through layer transitions.
- ❌ Click the **exit icon (top-right)** to quit.

---

