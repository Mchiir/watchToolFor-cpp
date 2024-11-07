# 🚀 C++ Project Automation with **Watchexec**

## 🔧 Problem Tip:
It can be tiresome to rebuild your project by running the same code repeatedly every time you make changes. Using automation tools like **watchexec** can save you time and effort by automatically rebuilding your project whenever you modify your code.

---

## 🎉 Welcome to Mchrispin's Guide!
Welcome to the official guide for using **watchexec** in your C++ projects. This guide is specifically designed for C++ programmers on Windows who use **g++** and **gcc** for compiling their code. You can also check out more projects by **Mchrispin** on [GitHub](https://github.com/Mchiir).

---

## 📝 Installation and Configuration Guide for Windows Users

### 1. 🍫 Installing **Chocolatey** (Windows Package Manager)
To begin, you’ll need to install **Chocolatey**, which is a package manager for Windows that will help you easily install `watchexec`, `make`, and other required tools.

1. Open **PowerShell** as **Administrator**.
2. Run the following command to install Chocolatey:
   ```powershell
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.SecurityProtocolType]::Tls12; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))