---
title: "SPARC OK Prompt Command Reference"
date: 2011-08-07T12:00:00Z
draft: false
tags: ["SPARC", "OK Prompt", "Reference"]
categories: ["Tech"]
---

The **SPARC OK prompt** is a powerful interface for troubleshooting and configuring SPARC-based systems. This reference provides a quick guide to commonly used commands.

---

### Accessing the OK Prompt

1. **From the operating system**:
   - Run the `init 0` command as root to drop to the OK prompt.

2. **From a cold start**:
   - Press the `Stop` key and `A` simultaneously during boot-up.

---

### Common Commands

| Command            | Description                               |
|--------------------|-------------------------------------------|
| `printenv`         | Displays all system environment variables. |
| `setenv <var> <val>` | Sets an environment variable.            |
| `reset`            | Resets the system.                       |
| `boot`             | Boots the system from the default boot device. |
| `boot <device>`    | Boots the system from a specified device. |
| `probe-scsi`       | Probes SCSI devices connected to the system. |
| `devalias`         | Lists device aliases.                    |
| `show-devs`        | Displays all devices on the system.      |
| `ok help`          | Displays general help information.       |

---

### Useful Tips

- Use `banner` to display system information, including the firmware version and Ethernet address.
- Use `test <device>` to perform diagnostics on a specific device.

---

### Reset Commands

| Command               | Description                             |
|-----------------------|-----------------------------------------|
| `reset-all`           | Performs a system-wide reset.          |
| `sync`                | Synchronizes system files before rebooting. |
| `power-off`           | Powers down the system.                |

---

For more detailed information, refer to the official SPARC documentation or online resources. The OK prompt is a crucial tool for troubleshooting and managing SPARC systems effectively.
