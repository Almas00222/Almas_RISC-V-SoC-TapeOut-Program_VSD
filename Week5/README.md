# 🧠 VSD Hardware Design Program  
## OpenROAD Installation & Usage Guide  

### 📘 Overview  

**OpenROAD** (Open Rapid Object-Oriented ASIC Design) is a complete open-source **RTL-to-GDSII** flow for digital IC design.  
It automates the backend design stages — from **synthesis, floorplanning, placement, routing,** to **layout generation** — allowing fast design iterations for both research and prototyping.

---

## 🚀 Installation Guide  

### 🧩 Steps to Install OpenROAD and Run the GUI  

#### 1️⃣ Clone the Repository  

Clone the official repository (with all submodules):  
```bash
git clone --recursive https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts
cd OpenROAD-flow-scripts
```
#### 2️⃣ Run the Setup Script
Execute the setup script to install dependencies and prepare the environment:

```bash
sudo ./setup.sh
```

#### 3️⃣ Build OpenROAD
After setup, build OpenROAD locally:

```bash
./build_openroad.sh --local
```

#### 4️⃣ Verify the Installation
Source the environment and verify that the tools are available:

```bash
source ./env.sh
yosys -help
openroad -help
```


#### 5️⃣ Run the OpenROAD Flow
Run the full RTL-to-GDSII flow:

```bash
cd flow
make
```

#### 6️⃣ Launch the GUI
To visualize the final layout in the GUI:

```bash
make gui_final
```

✅ Done! You’ve successfully set up OpenROAD and can now explore the full digital IC design flow.

🗂️ Directory Structure & File Descriptions
📁 OpenROAD-flow-scripts/
```plaintext
Copy code
├── docker           -> Docker setup files and scripts  
├── docs             -> Documentation for OpenROAD and flow scripts  
├── flow             -> Core files for running the RTL-to-GDSII flow  
├── jenkins          -> Regression and continuous integration test setup  
├── tools            -> Source/build tools required for the flow  
├── etc              -> Dependency installation scripts and utilities  
├── setup_env.sh     -> Script that sets up environment variables and paths
```
📁 Inside the flow/ Directory
```plaintext
Copy code
├── design      -> Example RTL-to-GDSII designs across multiple nodes  
├── makefile    -> Main makefile controlling the automated flow  
├── platform    -> Technology libraries (LEF, LIB, GDS, etc.)  
├── tutorials   -> Example projects and guided exercises  
├── util        -> Helper utilities and small tools  
├── scripts     -> Automation scripts for the flow  
```
