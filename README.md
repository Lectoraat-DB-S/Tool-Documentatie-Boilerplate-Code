# 🛠️ Tool Documentation & Boilerplate Code

**Central repository for hardware initialization, default configurations, and usage snippets.**


## 📖 Overview
This repository serves as the "Source of Truth" for interacting with the hardware tools used in our projects (Cameras, PLCs, Sensors, Microcontrollers, etc.). 

**The goal is to:**
1. **Standardize:** Ensure everyone initializes a specific camera or PLC the same way.
2. **Speed Up:** Provide copy-paste ready code blocks to get hardware running in minutes.
3. **Document:** Record known quirks, required firmware versions, and network settings.

## 📂 Repository structure
We organize tools by **Category** > **Manufacturer** > **Model**.

    tool-documentation/
    ├── 📷 Cameras/
    │   └── Basler/
    ├── 🤖 Robots/
    │   ├── ABB/
    │   ├── IGUS/
    │   └── UR/
    ├── 💻 PLCs/
    │   ├── Beckhoff/
    │   ├── PLCnext/
    │   └── Siemens/
    ├── 📡 Sensors/
    │   ├── Keyence/
    │   └── SICK/
    └── 📄 README.md

## 🤝 How to contribute
Found a new way to optimize a driver? Added a new sensor to the company stack? Please contribute! Because of permission settings, the process differs depending on your role.

### For Staff
*If you have **write** access to this repository*

1. **Create a branch:** `feature/add-new-sensor-name`.
2. **Add your folder:** Follow the structure: `Category/Manufacturer/Model`.
3. **Include three things:**
    * `boilerplate_code`: The code to make it run.
    * `README.md` (specific to that tool): Pinouts, voltage requirements, link to official PDF manual.
    * `requirements.txt`: Any software dependencies.
4. **Submit a pull request:** Assign a reviewer from the admin team

### For students
*If you have **Read-Only** access to this repository*

**Option 1: Fork & Pull request**

*This is the standard open-source workflow.*
1. **Create a fork:** Click the `Fork` button (top right of this page) to create a copy of this repo under your own account.
2. **Add your folder:** Follow the structure: `Category/Manufacturer/Model`.
3. **Include three things:**
    * `boilerplate_code`: The code to make it run.
    * `README.md` (specific to the tool): Pinouts, voltage requirements, link to official PDF manual.
    * `requirements.txt`: Any software dependencies.
4. **Create pull request:** Go to the `Pull Requests` tab, click `New Pull Request`, set `Compare across forks` and Select your fork as the source.

**Option 2: Contact your counselor or supervisor**

*If you are not comfortable with Git forks*
1. **Zip the following three things:**
    * `boilerplate_code`: The code to make it run.
    * `README.md` (specific to the tool): Pinouts, voltage requirements, link to official PDF manual.
    * `requirements.txt`: Any software dependencies.
2. **Send the zip to your supervisor:** Ask your supervisor to review and merge the code to the repository.
