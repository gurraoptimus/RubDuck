# RubDuck: Change Wallpaper 

## Description
This payload is designed to automate changing the desktop wallpaper on a Windows machine to an image downloaded from a specific URL. It uses PowerShell commands executed via the command prompt to achieve this functionality.

**Note:** Use this script responsibly and only in environments where you have explicit permission.

---

## How It Works
1. **Run Command Execution**:
   - Opens the Windows Run dialog (`GUI r`) to initiate a command.
2. **Command Prompt Launch**:
   - Launches the command prompt (`cmd`) and opens PowerShell.
3. **Download Wallpaper**:
   - Downloads an image from the specified URL (`https://gurraoptimus.se/img/github.jpg`).
4. **Set Wallpaper**:
   - Saves the image to a temporary directory and updates the Windows registry to set it as the wallpaper.
   - Refreshes the system parameters to apply the changes immediately.
5. **Loop for 60 Seconds**:
   - Ensures the wallpaper is refreshed every second for a minute.
6. **Cleanup**:
   - Closes the command prompt using `taskkill` to tidy up.

---

## Download Payload inject.bin
```vbscript
iwr -Uri https://raw.githubusercontent.com/gurraoptimus/RubDuck/refs/heads/main/inject.bin -OutFile C:\Users\User\Desktop\inject.bin
```

---

## Requirements
- **Hardware**: USB Rubber Ducky or compatible device.
- **Target System**: Windows operating system.
- **Tools**: DuckEncoder or a similar tool to compile the payload.

---

## Installation
1. Copy the above script into a `.txt` file.
2. Use DuckEncoder to convert the script into a binary `.bin` file.
   ```bash
   java -jar duckencoder.jar -i payload.txt -o inject.bin
   ```
3. Load the `inject.bin` file onto your USB Rubber Ducky.
4. Insert the USB Rubber Ducky into the target machine.

---

## Disclaimer
This script is intended for educational purposes only. Unauthorized use of this payload may violate laws and regulations. The author is not responsible for any misuse of this code.

---
- **Developer**: GurraOptimus
- **Website**: [GurraOptimus](https://www.gurraoptimus.se)
- **GitHub**: [GurraOptimus](https://github.com/gurraoptimus/)
- **Support Email**: support@gurraoptimus.se
