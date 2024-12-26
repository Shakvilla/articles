---
title: "3. A Practical Guide To Getting Up and Running With JavaScript"
datePublished: Fri Dec 09 2022 06:00:42 GMT+0000 (Coordinated Universal Time)
cuid: clbg3nfff0cfz01nv46af5qfp
slug: 3-a-practical-guide-to-getting-up-and-running-with-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1670536678332/eFqeqCfxS.png
tags: javascript, beginners, frontend-development

---

## **Running Javascript using Web Developer Tools**

Javascript is used to power modern web browsers. Every web browser includes the most recent stable JavaScript version. This allows web browsers to run Javascript code embedded in web applications.

In this lesson, I'll show you how to use the most popular web browsers on the Internet to run, write, and execute Javascript code in the browser. Don't worry if your chosen browser isn't covered in this article; the principles we'll utilize here are applicable to the vast majority of modern browsers. You only need to search for developer tools in the browser to get started. The following browsers will be discussed: Google Chrome, Mozilla Firefox, Safari, Microsoft Edge, and Brave Browser.

### **Google Chrome and Brave Browser**

Google Chrome is one of the most popular browsers, and it has earned the hearts of many developers. If you don't already have Google Chrome installed and operating on your machine, please do so before we continue.

Once you have Google Chrome installed, it comes with dev tools already whipped into the browser, so we are just going straight into where we can find the Chrome browser console.

There are two ways you can navigate to the console;

*   Using the keyboard shortcuts to open the dev console. To do this, you need to open your Chrome browser first, then press `F12` on windows OS or `Cmd+Opt+J` on Mac. This will open the developer tools console directly and it will be like this;
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670537770775/OMxBk9fTk.png align="left")
    
*   Before we start typing code, let me show you the other way to get to the dev console. Open your chrome browser, right-click or double-click on your mouse or mouse pad, and now click on `inspect` on the popup like in the picture below;
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670537978895/D00LX2G6f.png align="center")

Now the developer tools will open; click on the console tab. This will take you to the dev tools console.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670538189711/NAMtAxhmq.png align="left")

Now we are ready to start typing Javascript in the browser.

For example; let's try to print out a simple “Hello World” message in the console. Copy the code below and paste it into the console.

**Note**: Ignore the message “Console was cleared” in my console. I have a couple. chrome extensions, which add some Javascript code to the console once I open it, so to have a clean slate for this tutorial, I had to clear them. If you see a bunch of Javascript code in your console and wish to clear it, Run`clear()` and press enter, this will clear the console for you.

```javascript
console.log("Hello World!")
```

Now press `Enter` or `return` on your keyboard. The results will be `Hello World!` . Don’t worry if you don’t understand how the code works, in this course, I will have an in-depth discussion with you on how this whole thing works.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670538826349/gKPNp-X7C.png align="left")

### **Firefox and Edge**

*   To use keyboard shortcuts to open the console on Firefox and Edge, press `Ctrl + Shift+ I` or `F12` on Windows and Linux, or `Cmd+Opt+I` on macOS.
    
*   Or open a new empty tab on your browser, right-click or double-click on your mouse or mouse pad respectively, and select inspect on the popup, once the dev tools open, navigate to the console tab. You will arrive at the dev console. See the image below;
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670539526704/s8QyLHQnc.png align="left")
    

### **Running Javascript on a code editor:**

In this section, we shall go through how you can install and run Javascript on the code editor, and the code editor I will use is [Visual Studio Code](https://code.visualstudio.com/). Let me state clearly that, Visual Studio Code is just a personal preference, there are other good code editors out there that you can use. Other excellent editors include;

*   [Atom](https://atom.io/)
    
*   [Webstorm](https://www.jetbrains.com/webstorm/)
    
*   [Notepad++](https://notepad-plus-plus.org/)
    
*   [Vim](https://www.vim.org/)
    
*   [GNU Emac](https://www.gnu.org/software/emacs/)
    
*   [Sublime Editor](https://www.sublimetext.com/)
    
*   [Brackets](http://brackets.io/)
    

Feel free to use the editor of your choice and follow along. However, Webstorm editors might have a different approach to working with Javascript files. Set it up by reading the JetBrains documentation.

Javascript files take the extension. `.js`Once you create a file with the extension, you can write Javascript code in that file and run it on the browser or node server. Based on this, you can decide to use a normal text editor on Windows to write Javascript, but this is not advisable, as you will lose the good stuff (**syntax highlighting, Code completion, colored code, etc.)** that code editors provide.

### **Install Visual Studio Code**

> Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages and runtimes (such as C++, C#, Java, Python, PHP, Go, .NET).

![Example Page of how VSCode Looks like](https://cdn.hashnode.com/res/hashnode/image/upload/v1670551623937/AyKnoXZ94.png align="left")

The Microsoft team has in-depth documentation on VS Code. Click on the link below to visit the docs page. [*Visual Studio Code Docs Website.*](https://code.visualstudio.com/docs)

VS Code has support for Windows, Mac and Linux machines. Click on this [link](https://code.visualstudio.com/download) to download the supported version for your machine.

*   **Windows**
    
    1.  Download the [Visual Studio Code installer](https://go.microsoft.com/fwlink/?LinkID=534107) for Windows.
        
    2.  Once it is downloaded, run the installer (VSCodeUserSetup-{version}.exe). This will only take a minute.
        
    3.  By default, VS Code is installed under `C:\\Users\\{Username}\\AppData\\Local\\Programs\\Microsoft` VS Code.
        
    
    Alternatively, you can also download a [Zip archive](https://code.visualstudio.com/docs/?dv=winzip), extract it and run Code from there.
    
    **Tip:** Setup will add Visual Studio Code to your `%PATH%`, so from the console, you can type 'code .' to open VS Code in that folder. You will need to restart your console after the installation for the change to the %PATH% environmental variable to take effect. [Read more](https://code.visualstudio.com/docs/setup/windows)
    
    *   **Mac**
        
        1.  [Download Visual Studio Code](https://go.microsoft.com/fwlink/?LinkID=534106) for macOS
            
        2.  Open the browser's download list and locate the downloaded app or archive.
            
        3.  If archive, extract the archive contents. Use double-click for some browsers or select the 'magnifying glass icon with Safari.
            
        4.  Drag Visual Studio Code.app to the Applications folder, making it available in the macOS Launchpad.
            
        5.  Open VS Code from the **Applications** folder, by double-clicking the icon.
            
        6.  Add VS Code to your Dock by right-clicking on the icon, located in the Dock, to bring up the context menu and choosing **Options, Keep in Dock**.
            
            **Launching from the command line.**
            
            You can also run VS Code from the terminal by typing 'code' after adding it to the path:
            
            1.  Launch VS Code.
                
            2.  Open the **Command Palette** `Cmd+Shift+P` and type 'shell command' to find the Shell Command: `Install the 'code' command in PATH` command.
                
                ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670553113723/W1OGtRV32.png align="left")
                
            3.  Restart the terminal for the new `$PATH` value to take effect. You'll be able to type `code .` in any folder to start editing files in that folder
                
                > **Note**: If you still have the old code alias in your `.bash_profile` (or equivalent) from an early VS Code version, remove it and replace it by executing the Shell Command: `Install 'code'` command in the PATH command.
                
    *   **On Linux**
        
        See the [Download Visual Studio Code](https://code.visualstudio.com/download) page for a complete list of available installation options. By downloading and using Visual Studio Code, you agree to the [license terms](https://code.visualstudio.com/license) and [privacy statement](https://go.microsoft.com/fwlink/?LinkID=528096&clcid=0x409).
        
        **Debian and Ubuntu-based distributions**
        
        The easiest way to install Visual Studio Code for Debian/Ubuntu-based distributions is to download and install the [.deb package (64-bit)](https://go.microsoft.com/fwlink/?LinkID=760868), either through the graphical software center if it's available, or through the command line with:
        
        ```bash
        sudo apt install ./<file>.deb
        
        # If you're on an older Linux distribution, you will need to run this instead:
        # sudo dpkg -i <file>.deb
        # sudo apt-get install -f # Install dependencies
        ```
        
        Note that other binaries are also available on the [VS Code download page](https://code.visualstudio.com/Download).
        
        Installing the .deb package will automatically install the apt repository and signing key to enabling auto-updating using the system's package manager. Alternatively, the repository and key can also be installed manually with the following script:
        
        ```bash
        sudo apt-get install wget gpg
        wget -qO- <https://packages.microsoft.com/keys/microsoft.asc> | gpg --dearmor > packages.microsoft.gpg
        sudo install -D -o root -g root -m 644 packages.microsoft.gpg /etc/apt/keyrings
        sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/keyrings/packages.microsoft.gpg] <https://packages.microsoft.com/repos/code> stable main" > /etc/apt/sources.list.d/vscode.list'
        rm -f packages.microsoft.gpg
        ```
        
        Then update the package cache and install the package using:
        
        ```bash
        sudo apt install apt-transport-https
        sudo apt update
        sudo apt install code # or code-insiders
        ```
        
        **RHEL, Fedora, and CentOS-based distributions**
        
        We currently ship the stable 64-bit VS Code in a yum repository, the following script will install the key and repository:
        
        ```bash
        sudo rpm --import <https://packages.microsoft.com/keys/microsoft.asc>
        sudo sh -c 'echo -e "[code]\\nname=Visual Studio Code\\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\\nenabled=1\\ngpgcheck=1\\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
        ```
        
        Then update the package cache and install the package using `dnf` (Fedora 22 and above):
        
        ```bash
        dnf check-update
        sudo dnf install code
        ```
        
        Or on older versions using `yum`:
        
        Due to the manual signing process and the system we use to publish, the yum repo may lag behind and not get the latest version of VS Code immediately.
        
        **Snap**
        
        Visual Studio Code is officially distributed as a Snap package in the [Snap Store](https://snapcraft.io/store):
        
        You can install it by running:
        
        ```bash
        sudo snap install --classic code # or code-insiders
        ```
        
        Once installed, the Snap daemon will take care of automatically updating VS Code in the background. You will get an in-product update notification whenever a new update is available.
        
        **Note:** If `snap` isn't available in your Linux distribution, please check the following [Installing snapd guide](https://docs.snapcraft.io/installing-snapd), which can help you get that set up.
        
        Learn more about snaps from the [official Snap Documentation](https://docs.snapcraft.io/).
        
        **openSUSE and SLE-based distributions**
        
        The yum repository above also works for openSUSE and SLE-based systems, the following script will install the key and repository:
        
        ```bash
        sudo rpm --import <https://packages.microsoft.com/keys/microsoft.asc>
        sudo sh -c 'echo -e "[code]\\nname=Visual Studio Code\\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\\nenabled=1\\ntype=rpm-md\\ngpgcheck=1\\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/vscode.repo'
        ```
        
        Then update the package cache and install the package using:
        
        ```bash
        sudo zypper refresh
        sudo zypper install code
        ```
        
        **AUR package for Arch Linux**
        
        There is a community-maintained [Arch User Repository package for VS Code](https://aur.archlinux.org/packages/visual-studio-code-bin).
        
        To get more information about the installation from the AUR, please consult the following wiki entry: [Install AUR Packages](https://wiki.archlinux.org/index.php/Arch_User_Repository#Build_and_install_the_package).
        
        **Nix package for NixOS (or any Linux distribution using Nix package manager)**
        
        There is a community-maintained VS Code [Nix package](https://github.com/NixOS/nixpkgs/blob/master/pkgs/applications/editors/vscode/vscode.nix) in the nixpkgs repository. In order to install it using Nix, set `allowUnfree` option to true in your `config.nix` and execute:
        
        ```bash
        nix-env -i vscode
        ```
        
        **Installing .rpm package manually**
        
        The [VS Code .rpm package (64-bit)](https://go.microsoft.com/fwlink/?LinkID=760867) can also be manually downloaded and installed, however, auto-updating won't work unless the repository above is installed. Once downloaded it can be installed using your package manager, for example with `dnf`:
        
        ```bash
        sudo dnf install <file>.rpm
        ```
        
        Note that other binaries are also available on the [VS Code download page](https://code.visualstudio.com/Download).
        
        Note: This part of the book is from the Visual Studio Code Docs page at the time of writing this book. I recommend that you check the official docs page to make sure you are working latest updates of the docs