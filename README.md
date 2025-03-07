# Biometric Bypass Module

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/dfcf1c46fa474099a3aef3f5b3dfe8c3)](https://app.codacy.com/gh/rafagale/biometric-bypass?utm_source=github.com&utm_medium=referral&utm_content=rafagale/biometric-bypass&utm_campaign=Badge_Grade)

![GitHub stars](https://img.shields.io/github/stars/rafagale/biometric-bypass?style=social)
![GitHub downloads](https://img.shields.io/github/downloads/rafagale/biometric-bypass/total)
![GitHub Release (latest by date)](https://img.shields.io/github/v/release/rafagale/biometric-bypass)

## Overview

The Biometric Bypass Module is an Xposed module built on LSPosed's Modern Xposed API. It streamlines the face authentication process by automatically bypassing the confirmation step that follows a successful face unlock, providing a seamless, hands-free user experience.

## How It Works

The Biometric Bypass Module automates the manual confirmation step required after face authentication by the BiometricPrompt API, streamlining the process for a smoother user experience. Since it hooks into a System UI method, it works universally for all apps that don't override the default Android behavior. It also functions securely with apps protected by Magisk deny lists, Magisk Hide, or Shamiko.

## Visual Example

Below are visual examples comparing the experience with the Biometric Bypass Module enabled versus the default Android behavior:

<p align="center">
    <img src="media/module_disabled.gif" width="200" alt="Default Behavior">
    <br/>
    <strong>Default Behavior: Face unlock with manual confirmation required.</strong>
    <br/><br/>
    <img src="media/module_enabled.gif" width="200" alt="Module Enabled">
    <br/>
    <strong>Module Enabled: Face unlock with automatic confirmation bypass.</strong>
</p>

## Compatibility

- **Android Version:** 11 and above
- **Tested on:**
  - Pixel 8 Pro (husky) with Android 14 (Build: ap2a.240805.005)
  - Pixel 9 Pro (caiman) with **Android 15** (Build: AP3A.241005.015, Oct 2024)

## Installation Instructions

1. Ensure [LSPosed](https://github.com/mywalkb/LSPosed_mod/releases) is installed on your device.
2. Download and install the Biometric Bypass Module APK.
3. Activate the module via LSPosed.
4. Restart the System UI to apply changes.

## Additional Flavors

This module is also available for legacy Xposed API implementations:

- **[Legacy Xposed API (Java)](https://github.com/rafagale/biometric-bypass/tree/legacy-xposed-java)**
- **[Legacy Xposed API (Kotlin)](https://github.com/rafagale/biometric-bypass/tree/legacy-xposed-kotlin)**

## Risks and Warnings

Automating the confirmation step after biometric authentication could reduce security and lead to unintended actions. Carefully consider these risks before using the module.

## Contributions

Contributions and suggestions for improvement are welcome. If you have ideas or encounter issues, feel free to submit a pull request or open an issue.

## Disclaimer

This module modifies system behavior and may impact device security. Use it at your own risk.
