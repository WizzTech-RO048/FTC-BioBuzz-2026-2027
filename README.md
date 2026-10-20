<div align="center">

# 🤖 WizzTech — Team #19094

### *FIRST* Tech Challenge robot code · BIOBUZZ Season (2026–2027)

[![FTC Team 19094](https://img.shields.io/badge/FTC%20Team-19094-8C1B2C?style=flat-square&logo=first-tech-challenge&logoColor=white)](https://www.firstinspires.org/robotics/ftc/team-finder?team_number=19094)
[![Season](https://img.shields.io/badge/Season-BIOBUZZ%202026--2027-2E5BFF?style=flat-square)](https://www.firstinspires.org/robotics/ftc)
[![Language](https://img.shields.io/badge/Language-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://ftc-docs.firstinspires.org/programming_resources/android_studio_java/Android-Studio-Tutorial.html)
[![SDK](https://img.shields.io/badge/FTC%20SDK-v12.0-6C757D?style=flat-square)](https://github.com/FIRST-Tech-Challenge/FtcRobotController/releases)
[![License](https://img.shields.io/badge/License-BSD--Style-lightgrey?style=flat-square)](LICENSE)

**Liceul Teoretic „Grigore Moisil” · Romania 🇷🇴**

</div>

---

## 📖 About

This repository contains the source code of our **FTC Driver Station and Robot Controller** apps for the
**BIOBUZZ (2026–2027)** season. It is a working copy of the official
[FIRST Tech Challenge SDK](https://github.com/FIRST-Tech-Challenge/FtcRobotController) (v12.0), extended with
our own OpModes, subsystems, and autonomous routines written by team **#19094 — WizzTech**.

> [!NOTE]
> Everything under `FtcRobotController/` is stock SDK code. **All of our robot code lives in
> [`TeamCode/`](TeamCode/src/main/java/org/firstinspires/ftc/teamcode)** — start there.

## 🗂 Repository structure

| Path | What it is |
| --- | --- |
| [`TeamCode/`](TeamCode/) | ⭐ **Our code.** All OpModes, hardware classes, utilities, and autonomous programs |
| [`FtcRobotController/`](FtcRobotController/) | The official Robot Controller app and the SDK sample OpModes |
| [`docs/SDK-RELEASE-NOTES.md`](docs/SDK-RELEASE-NOTES.md) | Official FTC SDK release notes (v12.0 and earlier) |
| [`libs/`](libs/) | External libraries bundled with the SDK |
| [`doc/`](doc/) | SDK documentation resources |
| [`gradle/`](gradle/) · `build.gradle` | Gradle build configuration — touch only if you know what you're doing |

## 🚀 Getting started

### Requirements

- [Android Studio Narwhal 3 Feature Drop](https://developer.android.com/studio) or later
- A device (phone or Control Hub) with **FTC Robot Controller v11.0+** installed
- A team-configured Driver Station phone or tablet

### Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/WizzTech-RO048/FTC-BioBuzz-2026-2027.git
   cd FTC-BioBuzz-2026-2027
   ```

2. **Open it in Android Studio** — *File → Open* and select this folder (not a parent folder).

3. **Wait for Gradle to sync** — the first build downloads dependencies and takes a few minutes.

4. **Connect a device** via USB (enable USB debugging) or over Wi-Fi, then press **▶ Run** with the
   `FtcRobotController` configuration selected.

5. Build once more and run the app on the Driver Station device with the `TeamCode` configuration.

### Writing your first OpMode

1. Copy a sample from `FtcRobotController/java/org/firstinspires/ftc/robotcontroller/external/samples`
   into `TeamCode/java/org/firstinspires/ftc/teamcode` (right-click → Copy → Paste).
2. Rename the class, update the `@TeleOp` / `@Autonomous` name, and remove the `@Disabled` annotation.
3. Rebuild — your OpMode now appears in the Driver Station OpMode list.

See the [TeamCode readme](TeamCode/src/main/java/org/firstinspires/ftc/teamcode/readme.md) for a detailed
walkthrough, including the sample naming convention.

## 🧠 Useful resources

- 📚 [FTC Docs](https://ftc-docs.firstinspires.org/index.html) — tutorials for Blocks, OnBot Java, and Android Studio
- ☕ [FTC SDK Javadoc](https://javadoc.io/doc/org.firstinspires.ftc) — full API reference
- 💬 [FTC Community Forum](https://ftc-community.firstinspires.org/) — official support forum
- 📦 [SDK Releases](https://github.com/FIRST-Tech-Challenge/FtcRobotController/releases) — source archives and prebuilt APKs

## 👥 The team

<!-- Fill this in as the team grows! -->

| | |
| --- | --- |
| **Team number** | 19094 |
| **Name** | WizzTech |
| **School** | Liceul Teoretic „Grigore Moisil” |
| **Location** | Romania |
| **Program** | *FIRST* Tech Challenge |

## 📜 License & attribution

This project is derived from the [FTC SDK](https://github.com/FIRST-Tech-Challenge/FtcRobotController),
distributed by *FIRST* under the terms in [LICENSE](LICENSE).
FTC, *FIRST*, and related marks are trademarks of *FIRST*. This team is not affiliated with *FIRST*.

---

<div align="center">
<sub>Built with ⚡ by WizzTech #19094 — Go Wizz! 🧙</sub>
</div>
