# RDP Wrapper Library

**RDP Wrapper** is a lightweight, open-source solution that enables **concurrent Remote Desktop Protocol (RDP) sessions** on Windows systems — including editions like Home and Pro that typically restrict this functionality.

## 🔧 What It Does

RDP Wrapper acts as a **middle layer** between the Windows Terminal Services and the Remote Desktop Service (`termsrv.dll`). Instead of modifying system files directly, it **wraps around** them, allowing multiple users to establish simultaneous RDP connections without triggering licensing restrictions.

This is particularly useful for:

- IT administrators managing multiple remote sessions
- Developers testing multi-user environments
- Educational labs or training setups
- Home users needing remote access across devices

## ✅ Features

- 🧑‍💻 **Enables multiple concurrent RDP sessions**
- 🔒 **No system file patching required**
- 🖥️ **Supports Windows 10/11 Home and Pro**
- 🔄 **Easy to update and configure**
- 🧩 **Compatible with most Windows builds (with proper INI updates)**

## ⚠️ Disclaimer

> **Use at your own risk.**  
> RDP Wrapper is not officially supported by Microsoft. Its use may violate Windows licensing terms. Always ensure you're complying with your organization's IT policies and local laws.

## 📦 Installation

1. Clone or download this repository.
2. Run `install.bat` as Administrator.
3. Launch `RDPConf.exe` to verify configuration.
4. If needed, update `rdpwrap.ini` to support your Windows build.

> 💡 **Tip:** After Windows updates, check `RDPConf.exe` to ensure compatibility. You may need to update the `rdpwrap.ini` file manually.

## 🛠 Troubleshooting

- If `RDPConf.exe` shows `[not supported]`, your Windows build may require a newer `rdpwrap.ini`.
- Check the [community-maintained INI files](https://github.com/stascorp/rdpwrap/issues) for updates.
- Restart the RDP service or reboot after applying changes.

## 🤝 Contributing

Pull requests are welcome! If you’ve added support for a new Windows build or improved compatibility, feel free to contribute.

## 📄 License

This project is licensed under the MIT License.

---

**Maintained by IT engineers, for IT engineers.**  
RDP Wrapper is a powerful tool — use it responsibly and stay secure.
