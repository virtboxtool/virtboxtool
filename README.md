

<h1 align="center">🔐 VirtualBox Raw Disk + Ephemeral Mode</h1>
<p align="center">ViBox - Dual Boot, Sandbox & Anonymous Windows Execution</p>
 




<p align="center">
  <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="120"/>
</p>

[![Views](https://komarev.com/ghpvc/?username=your-github-username&style=flat-square&color=blue)](https://github.com/your-github-username)

---

## 📌 Project Description

This project demonstrates **advanced VirtualBox techniques** to run a **physically installed Windows system** as a **secure, disposable sandbox** using:

- **Raw Disk Access** (physical disk passthrough)  
- **Ephemeral Mode**  
- **Child / Differencing Image**  
- **Dual Boot Scenarios**  
- Secure and partially **anonymous Windows usage**

Ideal for:
- Security researchers  
- OSINT operations  
- Malware analysis  
- Software testing  
- Private virtualized experiments  

---

## 🧠 Key Technologies

<div align="center">
  <img src="https://github.com/devicons/devicon/blob/master/icons/windows8/windows8-original.svg" alt="Windows" width="40" height="40"/> &nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/linux/linux-original.svg" alt="Linux" width="40" height="40"/> &nbsp;
</div>

- VirtualBox  
- Raw Disk Access  
- Ephemeral Mode  
- Differencing Disk (Child Image)  
- Windows Sandbox  
- Dual Boot  
- Virtualization Security  
- Privacy & Anonymity  
- ViBox (USB Boot for VMs)  

---

## 💿 Raw Disk Access in VirtualBox

![VirtualBox raw disk access diagram](https://raw.githubusercontent.com/virtboxtool/virtboxtool/main/images/ViBoxhw.PNG)


**Raw Disk Access** enables a VM to use a **physical HDD/SSD directly** instead of a `.vdi` file.

### Capabilities:
- Boot an already installed Windows without reinstalling  
- Work with real disk partitions  
- Compatible with Dual Boot  

⚠️ **Caution:** Direct disk access is risky. Use **Ephemeral Mode** for safety.  

---

## 🧪 Ephemeral Mode & Child Image

![VirtualBox ephemeral mode child image](https://raw.githubusercontent.com/virtboxtool/virtboxtool/main/images/ViBoxEphermal.PNG)


**Ephemeral Mode** creates a temporary child image:

- Writes go to a **temporary differencing image**  
- Base disk remains **read-only**  
- VM shutdown **resets all changes**

**Child Image Benefits:**
- Intercepts writes  
- Prevents NTFS/FAT corruption  
- Safe for software & driver testing  

---

## ⚠️ Windows Host and VM Simultaneously

![Windows host and VM](https://raw.githubusercontent.com/virtboxtool/virtboxtool/main/images/Windows-11-VirtualBox.webp)

> Running the same Windows installation simultaneously on host & VM may corrupt the filesystem.

**Safe with this project if:**
- Ephemeral Mode is enabled  
- Child Image is used  
- No writable access to physical partition  
- Host OS is Windows  
- Windows boots from USB or another disk  

---

## 🔐 Windows as a Sandbox

![Windows sandbox VM](PATH_TO_IMAGE)

VirtualBox + Ephemeral Mode transforms Windows into:

- Disposable Sandbox  
- Secure Analysis Environment  
- Safe Testing Ground  

**Recommended Settings:**  
- Network: NAT / Host-Only  
- Clipboard & Drag & Drop: Disabled  
- USB Passthrough: Disabled  
- VPN inside Guest  
- Randomized MAC  

---

## 🕶 Anonymity & Privacy

![Anonymous Windows VM](PATH_TO_IMAGE)

Achieved through:

- Hardware virtualization  
- Isolation from host  
- Non-persistent changes  
- Reset on shutdown  

⚠️ Does **not guarantee absolute anonymity**, but increases privacy significantly.  

---

## 🔁 Dual Boot + VirtualBox

![Dual Boot Windows host Linux/Windows Guest](PATH_TO_IMAGE)

The same Windows installation can:

- Boot natively  
- Run inside VirtualBox  
- Be used as a Sandbox  

**Key:** Never allow simultaneous writable access.  

---

## 💾 Boot from USB or SystemDrive via ViBox

**ViBox** allows USB boot for VirtualBox VMs:

1. Launch ViBox & select USB drive  
2. Click **Create Virtual Disk**  
3. Create new VM in VirtualBox with the virtual disk  
4. Run the VM  

**Tested on:** Windows 7 / 8 / 10 / 11  

---
</div>
## 🔥 Stats & Links




<div align="center">
  <a href="https://linkedin.com/in/your-linkedin"><img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/></a>
  <a href="https://twitter.com/your-twitter"><img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/></a>
  <a href="https://youtube.com/your-channel"><img src="https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube Badge"/></a>
</div>


