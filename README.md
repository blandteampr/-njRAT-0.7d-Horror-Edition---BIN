README: njRAT 0.7d Horror Edition
Project Name: njRAT 0.7d Horror Edition
Version: 0.7d (Horror Branch)
Platform: .NET Framework (Windows)

Introduction
This repository contains the njRAT 0.7d Horror Edition, a highly modified and weaponized fork of the classic Bladabindi (njRAT) remote administration tool. Unlike its predecessor—which primarily focused on surveillance and remote access—this iteration is engineered for psychological dominance, system disruption, and demonstrative impact. It integrates legacy remote access capabilities with enhanced "horror" modules designed to intimidate, destabilize, and assert control over target systems.

The tool functions as a dual‑purpose payload: it retains standard RAT functionalities (remote desktop, keylogging, credential harvesting) while introducing destructive and harassment features that push it into the realm of cyber‑psychological operations. Its interface provides granular control over compromised machines, making it a comprehensive—though now largely dated—suite for penetration testing in controlled environments, forensic analysis of historical malware, and academic study of cyber‑threat evolution.

Disclaimer: This tool is published STRICTLY FOR EDUCATIONAL, RESEARCH, AND LEGITIMATE PENETRATION‑TESTING PURPOSES within fully authorized and isolated environments. Unauthorized use against any system without explicit permission is illegal and unethical.

Responsibility & Liability
Project Maintainer: PR

I, PR, expressly disclaim all responsibility and liability for any misuse, damage, or legal consequences arising from the deployment or study of this software. By accessing this repository, you acknowledge that:

<img width="1057" height="385" alt="image" src="https://github.com/user-attachments/assets/9a59b64b-9c5c-4e37-9938-38898b857269" />


<img width="171" height="509" alt="image" src="https://github.com/user-attachments/assets/9d53a2e9-e15a-4df4-a5a8-6d93e862675c" />


Manager → Opens the master control panel to manage all infected bots.

Run File → Executes any file or program remotely on the victim's machine.

Remote Desktop → Streams the victim's live screen for full remote control.

Remote Cam → Captures live video feed from the victim's webcam.

Microphone → Captures live audio from the victim's microphone.

Get Passwords → Harvests saved passwords from browsers and apps.

Grab Clipboard → Steals the current content of the victim's clipboard.

Fun → Accesses a submenu of harassment/prank modules.

Keylogger → Activates a background process to record every keystroke.

Open Chat → Opens a direct text chat window with the victim.

Ants → Covers the victim's screen with crawling insect animations.

Screenlocker → Locks the victim's screen, often with a ransom message.

Admin Privileges → Attempts to escalate malware permissions to Admin/System level.

Install → Installs the malware persistently (registry, startup).

Server → Opens configuration for the C&C server connection.

Power Options → Remotely shuts down, restarts, or logs off the victim's PC.

Open Folder → Opens a specific folder browser on the victim's file system.
====================================================================================
<img width="790" height="446" alt="image" src="https://github.com/user-attachments/assets/57cdbd0e-207a-4039-a119-369b28c45c22" />

njRAT 0.7d Horror Edition - Builder Interface Technical Breakdown
Builder: NORTH 07th HORROR EDITION

I. Connection & Server Configuration
Host/DNS: Sets the Command & Control (C&C) server IP/domain for the victim to connect back to.

Port: Specifies the C&C server port.

Connect with pastebin: Option to fetch C&C details (host:port) from a Pastebin raw URL for dynamic configuration.

II. Payload (Stub) Configuration & Evasion
Anti- Options:* Directives to detect and evade analysis environments.

Sorry, this application cannot run under a Virtual Machine – Terminates execution in virtualized/sandboxed environments.

Anti's – Likely "Anti-sandbox" or "Anti-debug" techniques.

Process Manipulation:

Kill process on run – Terminates specified processes (e.g., Wireshark.exe) upon execution.

Attempt kill Defender – Targets Windows Defender for disruption/disablement.

Persistence Mechanisms:
<img width="264" height="346" alt="image" src="https://github.com/user-attachments/assets/7242ef02-0d42-46f9-abc9-f3bd9d4f7dd8" />


Copy To StartUp – Copies payload to user's Startup folder.

Registry StartUp – Adds Registry run key for boot persistence.

Copy in Directory – Duplicates payload to a specified directory (%TEMP% or other).

Privilege Escalation & UAC Bypass:

Require Admin = Stub – Forces the payload to request Administrator privileges.

Disable UAC = Disabled – Option to attempt disabling User Account Control.
<img width="399" height="420" alt="image" src="https://github.com/user-attachments/assets/503b595b-4844-4db1-b110-fc4d2b0f650b" />


III. Stealth & Deception Modules
Fake Message Box: Fake MsgBox on run – Displays a decoy error/info message to the user upon execution.

Message Box Symbol: vbCritical, Warning, Info, Question – Sets the icon type.

Title/Message: Customizable box title and content.

Icon Changer: Masks the .exe with a benign/custom icon.

Assembly Changer: Alters internal .NET assembly metadata (version, description, etc.) to appear legitimate.

Hide = Disabled: Toggles process visibility/stealth mode.

IV. Harassment & Destructive Features ("Horror" Core)
BSOD on Kill Process: Triggers a Blue Screen of Death when terminating specified processes.

Screenlocker: MsgBox likely linked to a ransom lock-screen module.

Ants: Activates the visual screen-harassment animation.

Spread USB: Enables automatic infection of removable USB drives.

<img width="534" height="311" alt="image" src="https://github.com/user-attachments/assets/58479ed1-8f0a-4644-914f-c54812b2b01a" />


V. Logging & Data Collection
Keylogger logs in size KB: Sets the maximum file size for logged keystrokes before exfiltration.

VI. Binary Protection & Obfuscation (Packer/Protector Selection)
Pack on build: Selects a final executable packer/protector.

Options: Bland-Team, Themida, JET Reactor, RPX 4.0, Idlhost.exe (likely a protector alias).

Note: (Pick only one or breaks) – Mutually exclusive; using multiple corrupts the file.

VII. Build & Export
Build payload: Final button to compile the configured options into a working .exe binary.


