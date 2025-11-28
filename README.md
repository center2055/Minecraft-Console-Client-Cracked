<div align="center">

<img src="https://i.pics.rs/LLDhE.png" alt="Logo"/>

# Minecraft Console Client - Offline Fork

**This is a fork of [Minecraft Console Client (MCC)](https://github.com/MCCTeam/Minecraft-Console-Client) with offline account support.**

[Original Documentation](https://mccteam.github.io/) | [Download](#download) | [Installation](https://mccteam.github.io/guide/installation.html) | [Configuration](https://mccteam.github.io/guide/configuration.html) | [Usage](https://mccteam.github.io/guide/usage.html)

</div>

## **About This Fork ℹ️**

This fork adds **offline account support** to Minecraft Console Client, allowing you to connect to offline/cracked Minecraft servers without requiring Microsoft or Mojang authentication.

### **What's Changed**

- ✅ **New offline account type** - Connect with username/password to offline servers
- ✅ **Interactive account-type picker** - Choose account type on startup (microsoft/mojang/offline/yggdrasil)
- ✅ **Visible password prompt** - Password input is now visible (not hidden)
- ✅ **Auto `/login` command** - Automatically sends `/login <password>` after joining when in offline mode
- ✅ **Persistent account type** - Your account type choice persists across restarts

## **Download**

Get the latest release from the [Releases section](https://github.com/center2055/Minecraft-Console-Client-Cracked/releases/latest)

## **How to Use 📚**

### **Quick Start**

1. Run `MinecraftClient.exe`
2. When prompted for login, enter your username
3. Select account type: `offline` (or `microsoft`/`mojang`/`yggdrasil`)
4. Enter your password (visible input)
5. Enter server IP and port
6. The client will automatically send `/login <password>` after joining

### **Configuration File Option**

You can skip the interactive prompts by editing `MinecraftClient.ini`:

```ini
AccountType = "offline"
[Account]
Login = "your_username"
Password = "your_password"
```

### **Original Documentation**

For general usage, configuration, and features, see the [original MCC documentation](https://mccteam.github.io/):
- 📦 [Installation](https://mccteam.github.io/guide/installation.html)
- 📖 [Usage](https://mccteam.github.io/guide/usage.html)
- ⚙️ [Configuration](https://mccteam.github.io/guide/configuration.html)
- 🤖 [Chat Bots](https://mccteam.github.io/guide/chat-bots.html)
- 📝 [Sample configuration files](MinecraftClient/config/)

## **Technical Details**

### **Account Types**

- `microsoft` - Microsoft account authentication (default)
- `mojang` - Mojang account authentication
- `offline` - Offline/cracked server authentication (new)
- `yggdrasil` - Custom Yggdrasil authentication

### **Offline Mode Behavior**

- Generates a deterministic offline UUID based on username
- Skips online session validation
- Automatically sends `/login <password>` after successful join
- Password is required for offline mode

## **Original Project**

This is a fork of [Minecraft Console Client (MCC)](https://github.com/MCCTeam/Minecraft-Console-Client) by the MCC Team.

**Minecraft Console Client (MCC)** is a lightweight cross-platform open-source Minecraft TUI client for **Java** edition that allows you to connect to any Minecraft Java server, send commands and receive text messages in a fast and easy way without having to open the main Minecraft game.

## **License ⚖️**

Unless specifically stated, the code is from the MCC Team or Contributors, and available under CDDL-1.0. Else, the license and original author are mentioned in source file headers.

The main terms of the CDDL-1.0 license are basically the following:

-   You may use the licensed code in whole or in part in any program you desire, regardless of the license of the program as a whole (or rather, as excluding the code you are borrowing). The program itself may be open or closed source, free or commercial.
-   However, in all cases, any modifications, improvements, or additions to the CDDL code (any code that is referenced in direct modifications to the CDDL code is considered an addition to the CDDL code, and so is bound by this requirement; e.g. a modification of a math function to use a fast lookup table makes that table itself an addition to the CDDL code, regardless of whether it's in a source code file of its own) must be made publicly and freely available in source, under the CDDL license itself.
-   In any program (source or binary) that uses CDDL code, recognition must be given to the source (either project or author) of the CDDL code. As well, modifications to the CDDL code (which must be distributed as source) may not remove notices indicating the ancestry of the code.

More info at http://qstuff.blogspot.fr/2007/04/why-cddl.html
Full license at http://opensource.org/licenses/CDDL-1.0
