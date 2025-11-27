# ⚡ iAxCrystalOptimizer

> **Place Crystals at the speed of light.**

A fork of the WalksyCrystal mod for Minecraft Fabric. It improves the placement and destruction speed of End Crystals, designed for PvP Crystal players seeking maximum speed.

[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.1--1.21.4-brightgreen.svg)](https://www.minecraft.net/)
[![Fabric](https://img.shields.io/badge/Fabric-0.16.0+-orange.svg)](https://fabricmc.net/)
[![Java](https://img.shields.io/badge/Java-21+-blue.svg)](https://www.oracle.com/java/)

---

## 📋 Features

### 🚀 Crystal Optimization
- **Ultra-Fast Placement**: Places End Crystals at optimized speeds
- **Enhanced Destruction**: Breaks crystals with minimal latency
- **Usage**: Use responsibly
- **Adaptive Packet Limit**: Automatically adjusts the packet limit based on your ping

### ⚙️ Configuration System
- **Multiple Modes**: Legit, Balanced, Performance.
- **Customizable Settings**: Adjust placement and destruction cooldowns to suit your needs
- **In-Game Commands**: Activate/deactivate the optimizer with simple commands
- **MidnightLib Integration**: Intuitive configuration interface

### 🎯 Technical Features
- **Server-Side Verification**: Proper validation to prevent desynchronization
- **Raycast Optimization**: Accurate detection of blocks and entities
- **Multi-Entity Support**: Compatible with End Crystals, Slimes, and Magma Cubes
- **Intelligent Cooldown**: Cooldown system that prevents excessive spam

---

## 📦 Installation

### Prerequisites
- **Minecraft**: 1.21.1 - 1.21.4
- **Fabric Loader**: 0.16.0 or higher
- **Java**: 21 or higher
- **Fabric API**: Latest version
- **MidnightLib**: Latest version

### Installation Steps

1. **Download the Mod**
   - Go to the [Releases](https://github.com/iAkcc/iAxCrystalOptimizer/releases) section
   - Or visit [Modrinth](https://modrinth.com/mod/iaxcrystaloptimizer)
   - Download the latest `.jar` file

2. **Install Dependencies**
   - Download [Fabric API](https://modrinth.com/mod/fabric-api)
   - Download [MidnightLib](https://modrinth.com/mod/midnightlib)

3. **Place the Files**
   - Open your `.minecraft/mods` folder
   - Place `iaxcrystaloptimizer-1.4.0.jar`, Fabric API, and MidnightLib in the folder

4. **Launch Minecraft**
   - Select the Fabric profile
   - Enjoy the mod!

---

## 🎮 Usage

### Available Commands

```
/iaxcrystal - Toggle the optimizer on/off
/iaxmode (legit,balanced,performance) - Swap the modes between (legit, balanced and performance)
/iaxstatus - Displays the currently selected mode
```

### Configuration Modes

| Mode | Placement Cooldown | Break Cooldown | Description |
|------|-------------------|----------------|-------------|
| **Vanilla** | 250ms | 250ms | Vanilla Minecraft behavior |
| **Legit** | 100ms | 100ms | Subtle improvement, hard to detect |
| **Balanced** | 50ms | 50ms | Balance between performance and legitimacy |
| **Aggressive** | 25ms | 25ms | Maximum performance (more detectable) |

### Controls

- **Right Click** (with crystal in hand): Places optimized crystals on obsidian/bedrock
- **Left Click** (looking at a crystal): Destroys crystals with reduced latency

---

## 🛠️ Building from Source

### Requirements
- JDK 21 or higher
- Git

### Steps

```bash
# Clone the repository
git clone https://github.com/iAkcc/iAxCrystalOptimizer.git
cd iAxCrystalOptimizer

# Build the project
./gradlew build

# The .jar file will be in build/libs/
```

---

## 🔧 Technical Configuration

### Adaptive Packet Limit System

The mod automatically adjusts the packet limit based on your ping:

```java
Ping < 50ms   → Limit: 3-4 packets
Ping 50-100ms → Limit: 2-3 packets
Ping > 100ms  → Limit: 1-2 packets
```

### Random Variation

To avoid detectable patterns, the mod adds a 30% random variation to the packet limit, making the behavior appear more human-like.

---

## 📝 Important Notes

> [!WARNING]
> This mod is designed for use on servers that allow client-side mods. **Use at your own risk** on servers with strict policies against PvP mods.

> [!IMPORTANT]
> The mod implements anti-detection measures, but does not guarantee that it is 100% undetectable on all servers. Always check the server rules before using.

> [!NOTE]
> The "Vanilla" mode is designed to be completely legitimate and should not be detectable, as it replicates vanilla Minecraft behavior.

---

## 🤝 Contributing

Contributions are welcome! If you want to improve the mod:

1. Fork the project
2. Create a branch for your feature (`git checkout -b feature/NewFeature`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/NewFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## 👤 Author

**iAxres**

- GitHub: [@iAkcc](https://github.com/iAkcc)

---

## 🙏 Acknowledgments

- **Walksy** - Thanks to Walksy for the Crystal Optimizer concept

---

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/iAkcc/iAxCrystalOptimizer?style=social)
![GitHub forks](https://img.shields.io/github/forks/iAkcc/iAxCrystalOptimizer?style=social)
![GitHub issues](https://img.shields.io/github/issues/iAkcc/iAxCrystalOptimizer)

---

<div align="center">

**⚡ Made with ❤️ by iAxres**

*"Place Crystals at the speed of light."*

</div>
