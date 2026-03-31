# Device hardening and secure configuration

Even with good passwords, antivirus and patching, devices can still be vulnerable if they are configured in a weak or inconsistent way.

Device hardening and secure configuration are about setting up laptops, desktops and servers so they expose as little attack surface as possible and follow a consistent, secure baseline.

---

## 1. What device hardening means (plain language)

In simple terms, **hardening** a device means:

- Turning off what you do not need.  
- Strengthening what you do need.  
- Making sure all devices follow the same secure baseline.

For small and medium businesses, this typically includes:

- Removing or disabling unnecessary software and services.  
- Changing default passwords and settings.  
- Enabling built‑in security features such as firewalls, disk encryption and screen locks.  
- Applying secure configuration settings once and reusing them across devices.

---

## 2. Why secure configuration matters for SMBs

Many attacks succeed not because a system is unpatched, but because it is **misconfigured**:

- Default passwords left in place on routers, printers or applications.  
- Unnecessary services listening on the network.  
- Devices without screen locks or disk encryption, easy to abuse if lost or stolen.  
- Inconsistent settings across devices, making it hard to manage risk.

Secure, standardized configurations:

- Reduce your attack surface.  
- Make incidents less likely and less severe.  
- Simplify troubleshooting, compliance and audits.

---

## 3. Basic hardening steps for user devices (laptops and desktops)

For company‑managed laptops and desktops, a simple hardening baseline can include:

1. **Change defaults**
   - Change default local administrator passwords (or disable default admin accounts if not needed).  
   - Remove or disable unused built‑in accounts.

2. **Remove unnecessary software**
   - Uninstall trialware, games and other non‑business applications where possible.  
   - Avoid users installing arbitrary software without approval or review.

3. **Enable host firewall**
   - Turn on the built‑in operating system firewall (for example, Windows Defender Firewall).  
   - Only allow inbound connections that are required for business use.

4. **Enforce screen lock**
   - Configure automatic screen lock after a short period of inactivity (for example, 5–15 minutes).  
   - Require a password, PIN or biometric to unlock.

5. **Enable disk encryption**
   - Use full‑disk encryption (for example, BitLocker on Windows, FileVault on macOS) on laptops and other portable devices.  
   - Protect encryption keys and recovery keys in a secure manner (for example, device management or password manager).

6. **Standardize browser and application settings**
   - Set secure defaults for browsers (for example, block dangerous downloads, enable safe browsing features).  
   - Configure office and PDF software to use safe defaults for macros and active content.

7. **Limit local admin rights**
   - Normal user accounts should not have local administrator rights unless strictly required.  
   - Provide separate admin accounts for IT staff and use them only when necessary.

---

## 4. Hardening servers and critical systems (high‑level)

Servers and critical systems need extra care. Even if you host services in the cloud, many of the same concepts apply:

- **Minimize services**
  - Only enable services and features required for the server’s role.  
  - Disable or remove default services that are not in use (for example, legacy protocols, unused management interfaces).

- **Restrict access**
  - Limit who can log on interactively or via remote access.  
  - Use firewalls and access control lists to restrict network access to required sources and ports.

- **Secure management interfaces**
  - Protect remote management (for example, SSH, RDP, web admin portals) with MFA, strong passwords and network restrictions.  
  - Avoid exposing management interfaces directly to the internet whenever possible.

- **Standard builds**
  - Use documented “golden images” or templates for servers with pre‑hardened configurations.  
  - Apply the same baseline to all servers of the same type.

- **Logging and monitoring**
  - Ensure important security‑relevant events are logged (for example, failed logins, admin changes, service restarts).  
  - Centralize or regularly review logs where possible.

---

## 5. Using baselines and benchmarks

To avoid configuring each device manually and differently, you should define one or more **secure configuration baselines**:

- A baseline is a documented set of:
  - Settings (for example, password policies, lockout policies, firewall rules).  
  - Installed software and versions.  
  - Enabled/disabled services and features.

For many small and medium businesses:

- You can start from vendor or community benchmarks (for example, CIS Benchmarks) and simplify them to match your environment and capacity.
- Apply these baselines through:
  - Group Policy or similar tools for domain‑joined Windows devices.  
  - Mobile device management (MDM) or endpoint management platforms.

The key is consistency: devices of the same type should be configured in the same secure way.

---

## 6. Relationship to other controls

Secure configuration works together with other controls you already have:

- **Patching and updates** – patches are most effective when applied on top of a hardened, standardized configuration.  
- **Antivirus and endpoint protection** – hardening reduces the number of ways malware can execute, while endpoint protection detects what still gets through.
- **Access control and least privilege** – device hardening enforces limits on what users and apps can do locally.

Think of hardening as “building a stronger wall and closing unneeded doors”, while other controls monitor, patch and defend what remains.

---

## 7. Practical steps to get started

For a small or medium business, you can start with a short, focused plan:

1. **List device types**
   - Identify main categories (for example, Windows laptops, macOS laptops, Windows servers, network devices).

2. **Define a minimal baseline per category**
   - Screen lock timeout.  
   - Disk encryption status.  
   - Firewall enabled.  
   - Default accounts and passwords changed.  
   - Local admin rights restricted.

3. **Implement through tools**
   - Use domain policies, MDM or endpoint management tools where available.  
   - For very small environments, document manual steps and apply them consistently.

4. **Check compliance**
   - Periodically verify that new and existing devices match the baseline (for example, through spot checks or reports from management tools).

5. **Improve over time**
   - Add more settings (for example, browser hardening, application allow‑listing) as your maturity grows.

---

## 8. Minimal checklist for device hardening

Use this checklist as a quick status check:

- [ ] We have a basic, documented secure configuration baseline for our main device types.  
- [ ] Default passwords and accounts have been changed or disabled on devices and key applications.  
- [ ] Built‑in host firewalls are enabled on laptops, desktops and servers (or alternative protections are documented).  
- [ ] Laptops and other portable devices use full‑disk encryption.  
- [ ] Automatic screen lock is enabled with a reasonable timeout.  
- [ ] Normal user accounts do not have local administrator rights by default.  
- [ ] Servers and critical systems have unnecessary services disabled and management interfaces restricted.  
- [ ] We periodically verify that devices conform to our baseline and update it when needed.

Unchecked boxes show where you can strengthen your device configuration and hardening over the next 30–90 days.
