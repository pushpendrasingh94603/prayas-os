# 🚀 Minimalist Arch-Based Custom Linux OS

A lightweight, efficient, and customizable Linux distribution built on Arch Linux, designed for **low-end and modern systems** with optimized performance, minimal resource usage, and flexible desktop environments.

---

## 📌 Overview

This project presents a **custom Arch Linux-based operating system** focused on:

- ⚡ Low RAM and CPU usage  
- 🚀 Faster boot times  
- 🧩 Minimal yet functional system design  
- 🖥️ GUI optimization for real-world use cases  

It is particularly useful for:

- Low-end / legacy computers  
- Educational systems  
- Exam environments  
- Lightweight personal computing  

The system leverages Arch Linux’s rolling release model to ensure **latest updates and security patches**.

---

## 🎯 Key Features

- 🪶 **Lightweight Design** – Minimal packages, optimized services  
- ⚡ **Fast Boot Time** – ~17–35 seconds depending on system  
- 💾 **Low RAM Usage**
  - XFCE variant: ~500–600 MB idle  
  - KDE variant: ~1–1.2 GB idle  
- 🧠 **Efficient Resource Management**
- 🔄 **Rolling Release (Arch-based)**
- 🎨 **Custom Branding & UI**
- 🔐 **User & Permission Management (Wheel group)**  
- 📦 **Pacman Package Manager**

---

## 🖥️ Variants

### 🟢 Type 1 – XFCE (Lightweight)
- Best for low-end hardware  
- Minimal RAM usage  
- Faster performance  

### 🔵 Type 2 – KDE Plasma (Feature-rich)
- Modern UI experience  
- More features  
- Slightly higher resource usage  

---

## 🏗️ Architecture & Components

| Component            | Technology Used |
|---------------------|----------------|
| Base System         | Arch Linux |
| Kernel              | Linux Kernel |
| Display Manager     | Lightdm / SDDM |
| Desktop Environments| XFCE4 / KDE Plasma |
| Package Manager     | pacman |
| Bootloader          | GRUB |

---

## ⚙️ Methodology

The OS is built using Arch Linux’s **releng profile and mkarchiso tools**.

### Steps:

1. Setup Arch-based host environment  
2. Configure releng profile  
3. Customize system:
   - Bootloader (GRUB / EFI)
   - Package list
   - pacman configuration  
4. Configure services:
   - NetworkManager  
   - Bluetooth  
   - SDDM  
5. User & permission setup  
6. Branding & system identity  
7. Cleanup unnecessary files  
8. Build ISO using `mkarchiso`  
9. Testing & performance validation  

---

## 📦 Essential Packages

### Core System
- base, linux, systemd, bash, sudo  
- pacman, glibc, mkinitcpio  

### Hardware & Drivers
- intel-ucode / amd-ucode  
- efibootmgr  

### Filesystem
- e2fsprogs, dosfstools  

### Networking
- iwd, dhcpcd, networkmanager  

### Desktop & GUI
- XFCE4 / KDE Plasma  
- xorg / Wayland  
- SDDM  

---

## 🧪 Performance Comparison

### 💾 RAM Usage (Idle)

| OS                  | RAM Usage |
|---------------------|----------|
| Custom OS (XFCE)    | ~521–599 MB |
| Custom OS (KDE)     | ~1000–1270 MB |
| Ubuntu              | ~1229–1843 MB |
| Windows             | ~2539–5101 MB |

---

### 🚀 Boot Time

| OS                  | Boot Time |
|---------------------|----------|
| Custom OS (XFCE)    | ~17–31 sec |
| Custom OS (KDE)     | ~18–35 sec |
| Ubuntu              | ~1–2.5 min |
| Windows             | ~44–135 sec |

---

### 💽 Disk Usage

| OS                  | Disk Usage |
|---------------------|----------|
| Custom OS (XFCE)    | ~7.8–11 GB |
| Custom OS (KDE)     | ~10–12 GB |
| Ubuntu              | ~11–13 GB |
| Windows             | ~55 GB |

---

## 🔍 Key Observations

- XFCE variant performs best on low-end systems  
- KDE variant balances performance and features  
- Ubuntu offers ease of use but higher resource usage  
- Windows shows highest resource consumption and slower performance  

This OS significantly improves usability of **older hardware systems**.

---

## 🛠️ Build Instructions

```bash
sudo ./custom_build.sh
sudo ./clean.sh
sudo ./build.sh
