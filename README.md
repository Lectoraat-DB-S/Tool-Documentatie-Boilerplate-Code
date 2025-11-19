# 🛠️ Tool Documentation & Boilerplate Code

**Central repository for hardware initialization, default configurations, and usage snippets.**


## 📖 Overview
This repository serves as the "Source of Truth" for interacting with the hardware tools used in our projects (Cameras, PLCs, Sensors, Microcontrollers, etc.). 

**The goal is to:**
1. **Standardize:** Ensure everyone initializes a specific camera or PLC the same way.
2. **Speed Up:** Provide copy-paste ready code blocks to get hardware running in minutes.
3. **Document:** Record known quirks, required firmware versions, and network settings.

## 📂 Repository Structure
We organize tools by **Category** > **Manufacturer** > **Model**.

    tool-documentation/
    ├── 📷 Cameras/
    │   ├── Basler/
    │   └── Cognex/
    ├── 🤖 PLCs/
    │   ├── Siemens/
    │   │   PLCnext/
    │   └── Beckhoff/
    ├── 📡 Sensors/
    │   ├── Keyence/
    │   └── SICK/
    └── 📄 README.md

## 🤝 How to Contribute
Found a new way to optimize a driver? Added a new sensor to the company stack? Please contribute! Because of permission settings, the process differs depending on your role.

### For Staff
*If you have **write** access to this repository*

1. **Create a Branch:** `feature/add-new-sensor-name`.
2. **Add Your Folder:** Follow the structure: `Category/Manufacturer/Model`.
3. **Include Three Things:**
    * `boilerplate_code`: The code to make it run.
    * `README.md` (specific to that tool): Pinouts, voltage requirements, link to official PDF manual.
    * `requirements.txt`: Any software dependencies.
4. **Submit a Pull Request:** Assign a reviewer from the admin team

### For students
*If you have **Read-Only** access to this repository*

**Option 1: Fork & Pull Request (Recommended)**

*This is the standard open-source workflow.*
1. Click the **Fork** button (top right of this page) to create a copy of this repo under your own account.
2. Add your code and documentation to **your** forked version.
3. Go to the **Pull Requests** tab.
4. Click "New Pull Request" -> set "Compare across forks" -> Select your fork as the source.

**Option 2: Contact your Counselor or Supervisor**

*If you are not comfortable with Git forks*
1. Zip your code folder (ensuring it follows the repository structure and contains the correct documents).
2. Send it to your project counselor or supervisor.
3. Ask them to review and merge it into the main branch.
