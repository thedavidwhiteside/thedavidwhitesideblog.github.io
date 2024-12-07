---
title: "Solaris Shutdown, Reboot, Init, and Halt Command Differences"
date: 2012-05-07T12:00:00Z
draft: false
tags: ["Solaris", "Commands", "Unix"]
categories: ["Tech"]
---

Solaris, like other Unix-based systems, offers multiple commands to manage system states such as shutting down, rebooting, and halting. Each command has specific use cases and functionality. Here’s a quick guide to the differences.

---

### Shutdown Commands Overview

| Command      | Functionality                                       |
|--------------|-----------------------------------------------------|
| `shutdown`   | Gracefully shuts down the system with warnings to users. |
| `reboot`     | Reboots the system immediately.                     |
| `init`       | Changes the system run level.                      |
| `halt`       | Stops the system without syncing disks.            |

---

### **1. `shutdown`**

The `shutdown` command is used to gracefully bring the system down while notifying logged-in users.

#### Example:
```bash
shutdown -i 5 -g 60 -y
