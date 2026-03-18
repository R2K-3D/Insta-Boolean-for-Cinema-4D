<div align="center">

# ⚡ Insta Boolean for Cinema 4D

[![Cinema 4D](https://img.shields.io/badge/Cinema%204D-Compatible-blue?style=for-the-badge&logo=maxon)](https://www.maxon.net/)
[![Python](https://img.shields.io/badge/Python-Script-yellow?style=for-the-badge&logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Downloads](https://img.shields.io/github/downloads/SPluzh/SPVideoCoursesPlayer/total)](https://github.com/SPluzh/SPVideoCoursesPlayer/releases)

*A set of Python scripts for Maxon Cinema 4D that significantly speeds up the workflow of creating and managing Boolean Generators.*

[Features](#-key-features) • [Installation](#%EF%B8%8F-installation) • [Usage](#-usage) • [Compatibility](#-compatibility)

</div>

---

## 🚀 The Set Includes

| Script | Operation | Description |
|---|:---:|---|
| `Insta_Subtract_v1.py` | <img width="64" height="64" alt="Insta_Substract_v1" src="https://github.com/user-attachments/assets/b47d9199-613c-4efa-a8ae-ccb53f80feb1" />| Creates a Boolean generator in **A Subtract B** mode. |
| `Insta_Union_v1.py` |<img width="64" height="64" alt="Insta_Union_v1" src="https://github.com/user-attachments/assets/754e59cc-8237-4618-93d7-c58b3e4c0552" />| Creates a Boolean generator in **A Union B** mode. |
| `Insta_Intersect_v1.py` |<img width="64" height="64" alt="Insta_Intersect_v1" src="https://github.com/user-attachments/assets/cad4e705-a23f-477e-a27c-5a01123e1154" />| Creates a Boolean generator in **A Intersect B** mode. |
| `Insta_Without_v1.py` |<img width="64" height="64" alt="Insta_Without_v1" src="https://github.com/user-attachments/assets/7c49465d-c55c-4611-ad8c-a7f71a8eb2d4" />| Creates a Boolean generator in **A Without B** mode. |

---

## ✨ Key Features

- ⚡ **Instant Creation**  
  Select two or more objects and run the script. It automatically places them into a new Boolean generator with the respective operation mode.

- 🌳 **Hierarchy Awareness**  
  The newly created Boolean generator is intelligently placed at the exact same location in the *Object Manager* hierarchy as your first selected object.

- 📐 **Transform Preservation**  
  Objects keep their exact global position, scale, and rotation when being nested under the Boolean generator.

- 🛡️ **Smart Filtering**  
  The scripts automatically filter out child objects if their parent is also selected, preventing duplicate hierarchy moves and unpredictable errors.

- 🔗 **Append to Existing Booleans**  
  If the first selected object is *already* a Boolean generator, the scripts will seamlessly add the other selected objects into it. If appending an operation that differs from the generator's main mode, it will automatically apply a **Boolean Tag** with the correct overriding mode!

- ⏪ **Full Undo/Redo Support**  
  Every action is fully registered in the Cinema 4D undo stack. Change your mind? Just hit `Ctrl+Z`.

<br>

## ⚙️ Installation

1. Open Cinema 4D.
2. Go to **Extensions -> User Scripts -> Script Folder...**  
   *(Or go to **Edit -> Preferences -> Open Preferences Folder** and navigate to the `library/scripts` folder)*.
3. Drop the `.py` script files into this folder.
4. Restart Cinema 4D or go to **Extensions -> User Scripts -> Reload Python Plugins**.
5. Customization: You can now drag these scripts into your custom UI palettes or assign hotkeys via the **Commander** `(Shift + 12)`.
6. Assign hot keys (more convenient) at your discretion

<br>

## 📖 Usage

### Standard Workflow
1. Select your target **Main Object (A)**.
2. Hold `Ctrl/Cmd` and click to select the **Target Objects (B, C...)**. 
   > ⚠️ ***Note:** Selection order matters! The very first object you clicked will act as the primary mesh.*
3. Run the preferred script (e.g., *Subtract*).
4. The Boolean generator is built instantly, keeping your scene perfectly organized!

### Advanced Workflow (Appending)
If you select an **existing Boolean generator** as your first object, running the script will *append* the additionally selected objects into that existing Boolean logic. Mix and match operations freely using the auto-generated Boolean Tags!

<br>

## 💻 Compatibility

Written specifically for the modern Python API in newer versions of Maxon Cinema 4D

---

<div align="center">
  <i>If you find these scripts helpful, feel free to star the repository! ⭐</i>
</div>
