# 📁 TeamCode — WizzTech #19094

This module is where **all of our robot code lives**. Never edit anything under `FtcRobotController/`
for team purposes — it gets overwritten on SDK updates. Our OpModes, hardware classes, and utilities
go in:

```
TeamCode/src/main/java/org/firstinspires/ftc/teamcode
```

Currently this folder is a clean slate — here's how to add your first OpMode.

---

## 🛠 Creating your own OpMode

The easiest way to start is to copy a sample OpMode and make it your own.

Samples live in the `FtcRobotController` module. In the Android Studio *Project/Android* tab, expand:

```
FtcRobotController/java/org/firstinspires.ftc.robotcontroller/external/samples
```

### Steps

1. Locate the desired sample class in the Project/Android tree.
2. Right-click the sample class and select **Copy**.
3. Expand the `TeamCode/java` folder.
4. Right-click `org.firstinspires.ftc.teamcode` and select **Paste**.
5. Give the copy a meaningful, capitalized class name (you'll add more similar classes later).

### Activating it on the Driver Station

Every sample starts with annotations like these:

```java
@TeleOp(name="Template: Linear OpMode", group="Linear Opmode")
@Disabled
```

- The text in `name="..."` is what appears in the Driver Station's OpMode list — rename it.
- The `group="..."` value keeps the OpMode list organized.
- **`@Disabled` hides the OpMode from the Driver Station** — delete or comment it out to enable it,
  then rebuild.

## 🏷 Naming convention of samples

Samples are named by prefix so you can tell at a glance what they do:

| Prefix | Meaning |
| --- | --- |
| `Basic` | Bare-bones skeleton of a particular OpMode style |
| `Sensor` | Shows the minimal code to read one specific sensor |
| `Robot` | Assumes a simple two-motor (differential) drive base; a drivable baseline or navigation example |
| `Concept` | Demonstrates one specific idea — may not drive a robot at all |

After the prefix:

- **Sensor** classes are `Sensor_Company_Type`
- **Robot** classes are `Robot_Mode_Action_OpModeType`
- **Concept** classes are `Concept_Topic_OpModeType`

Details are in `sample_conventions.md` in the
[samples folder](../../../../../../../../FtcRobotController/src/main/java/org/firstinspires/ftc/robotcontroller/external/samples).

## 🚨 Caution

- Don't put team-specific code in the SDK `samples` folder — copy samples out, then modify the copies.
- Keep OpMode names unique; duplicates clash in the Driver Station list.
- Don't modify `FtcRobotController` module code — an SDK update will overwrite it.

## 🧑‍🤝‍🧑 Advanced: cloning TeamCode for multiple teams

If several sub-teams share this repo and each needs its own module, clone `TeamCode` once per team so
every module can see the others' code while maintaining its own. This is **not for beginners**, it's done
outside Android Studio (close it first), and you should back up the project first.

1. Copy the whole `TeamCode` folder to a sibling folder, e.g. `Team0417`.
2. In the new `Team0417` folder, delete `TeamCode.iml`.
3. Rename `Team0417/src/main/java/org/firstinspires/ftc/teamcode` to `team0417` (lowercase `team`).
4. In `Team0417/src/main/AndroidManifest.xml`, change `package="org.firstinspires.ftc.teamcode"` to
   `package="org.firstinspires.ftc.team0417"`.
5. Add `include ':Team0417'` to `/settings.gradle`.
6. Reopen Android Studio and use **Build → Clean Project**.
