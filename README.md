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

After installation, verify that Chocolatey was successfully installed by running:

    choco --version

2. ⚡ Installing Watchexec

Now that Chocolatey is installed, you can easily install watchexec, which will monitor your project files for changes and automatically rebuild the project.

Install watchexec using Chocolatey:

    choco install watchexec

Verify the installation by checking the version:

    watchexec --version

3. 🛠 Installing Make

Make is essential for automating the build process. You can easily install it with Chocolatey as well.

Install make by running:

    choco install make

Verify the installation:

    make --version

📝 Creating Your Makefile

Now that the tools are installed, you need to create a Makefile to automate the compilation of your C++ project. In your project directory, create a file named 'Makefile' (without any extension) with the following content:

    # This is the default target
    all: main.exe

    # Rule to build main.exe from main.cpp
    main.exe: main.cpp
    # Compile main.cpp into an executable named main.exe
        g++ -o main.exe main.cpp

    # Clean target to delete the compiled executable
    clean:
        del main.exe

📚 Explanation:

    all: This is the default target. When you run make, it will attempt to build main.exe.
    main.exe: This rule compiles main.cpp into an executable file named main.exe using the g++ compiler.
    clean: This target is used to remove the compiled executable (main.exe) by running the del command.

🖥 Running Your Project with Watchexec

Now that everything is set up, you can use watchexec to automatically monitor file changes and trigger a rebuild every time you modify your code.
1. 💡 Using Watchexec (Automatic Rebuild on Code Change)

To automatically rebuild your project whenever you make changes to your main.cpp file, run the following command:

    watchexec -- make;

This command will watch your project directory for any changes in files and automatically re-run make to rebuild the project(main.cpp).
2. 🔨 Manual Build with Make

If you prefer to manually trigger the build process, you can use:

    make

This command will compile your project based on the instructions in the Makefile.

3. 🧹 Cleaning the Build

To remove the previously compiled main.exe file, you can use the clean target:

    make clean

This will delete the main.exe file.
⚠️ Troubleshooting

If you encounter any issues during installation or configuration, feel free to reach out for assistance. You can email me at: mugishachrispin590@gmail.com.

✋ Farewell and Happy Coding!

I hope this guide helps you automate your C++ project workflow, saving you time and effort while you focus on what matters most—coding. Happy programming! 🚀