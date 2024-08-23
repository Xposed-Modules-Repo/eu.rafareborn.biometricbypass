# Biometric Bypass Module

![GitHub stars](https://img.shields.io/github/stars/Xposed-Modules-Repo/es.rafagale.biometricbypass?style=social)
![GitHub downloads](https://img.shields.io/github/downloads/Xposed-Modules-Repo/es.rafagale.biometricbypass/total)
![GitHub Release Downloads](https://img.shields.io/github/downloads/Xposed-Modules-Repo/es.rafagale.biometricbypass/latest/total)
![GitHub Release (latest by date)](https://img.shields.io/github/v/release/Xposed-Modules-Repo/es.rafagale.biometricbypass)


## Overview

The Biometric Bypass Module is an Xposed module utilizing LSPosed's Modern Xposed API. It automatically bypasses the confirmation step following a successful face unlock, streamlining the authentication process for a hands-free user experience.

## How It Works

This module hooks into a System UI method responsible for managing the confirmation step after face authentication. By intercepting this process, the module automates the confirmation required by the new BiometricPrompt API, allowing users to proceed without additional input. This approach works universally across apps that rely on the default Android behavior and remains secure even in environments protected by Magisk deny lists, Magisk Hide, or Shamiko.

## Visual Example

<p align="center">
    <img src="https://raw.githubusercontent.com/rafagale/biometric-bypass/master/media/module_disabled.gif" width="200" alt="Default Behavior">
    <br/>
    <strong>Default Behavior: Face unlock with manual confirmation required.</strong>
    <br/><br/>
    <img src="https://raw.githubusercontent.com/rafagale/biometric-bypass/master/media/module_enabled.gif" width="200" alt="Module Enabled">
    <br/>
    <strong>Module Enabled: Face unlock with automatic confirmation bypass.</strong>
</p>


## Compatibility

- **Supported Android Versions:** 11 and above
- **Tested Device:** Pixel 8 Pro (husky) on Android 14 (Build: ap2a.240805.005)
- **Xposed Framework:** LSPosed

## Installation Instructions

1. Ensure [LSPosed](https://github.com/mywalkb/LSPosed_mod/releases) is installed.
2. Download and install the Biometric Bypass Module APK.
3. Activate the module in LSPosed.
4. Restart System UI to apply changes.

## Additional Flavors

Legacy versions are available for older Xposed APIs:

- **[Java Legacy Xposed API](https://github.com/rafagale/biometric-bypass/tree/legacy-xposed-java)**
- **[Kotlin Legacy Xposed API](https://github.com/rafagale/biometric-bypass/tree/legacy-xposed-kotlin)**

## Risks and Warnings

Automating the confirmation step can reduce security and lead to unintended actions. Use this module with caution.

## Contributions

Contributions are welcome. Submit a pull request or open an issue to help improve the module.

## Disclaimer

This module modifies system behavior and may impact device security. Use at your own risk.
