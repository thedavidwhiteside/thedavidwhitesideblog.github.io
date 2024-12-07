---
title: "Using a Smartcard (PIV or CAC) with Ansible"
date: 2024-12-07T12:00:00Z
draft: false
tags: ["Ansible", "Smartcard", "PIV", "CAC"]
categories: ["Tech"]
---

Integrating a smartcard, such as a Personal Identity Verification (PIV) or Common Access Card (CAC), into your Ansible workflows can enhance security by leveraging certificate-based authentication. This guide explains how to set up and use a smartcard with Ansible.

---

### **Prerequisites**

1. **Smartcard (PIV or CAC)**:
   - Ensure your smartcard is properly provisioned and contains the required certificates.

2. **Smartcard Reader**:
   - A compatible smartcard reader must be connected to your system.

3. **Required Tools**:
   - Install `opensc` and `pkcs11-tool`:
     ```bash
     sudo apt-get install opensc pcscd
     ```

4. **SSH Configuration**:
   - Ensure `ssh-agent` is running and configured to use the smartcard.

---

### **Step 1: Verify Smartcard Functionality**

Check that your system recognizes the smartcard by listing the available certificates:
```bash
pkcs11-tool --list-slots
