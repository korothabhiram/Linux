# 🐧 WSL – Windows Subsystem for Linux

Ever wished for the best of both worlds—Windows and Linux—without the hassle of dual-booting or managing virtual machines? Enter **Windows Subsystem for Linux (WSL)**: a nifty feature that lets you run a Linux environment directly on your Windows machine.

> “Because sometimes, you just want to `sudo` while staying in your Windows comfort zone.”

🔗 [Learn more about WSL](https://learn.microsoft.com/en-us/windows/wsl/about)

---

## 🧑‍💻 My WSL Journey

I jumped on the WSL bandwagon when it first rolled out. The idea of running Linux on Windows without the overhead of dual-booting or virtual machines was too enticing to pass up. Plus, for my command-line needs, it was a game-changer.

Later, I ventured into using WSL professionally, especially for running Terraform plans. Encountered a few hiccups—browser authentication with Azure AD was a bit finicky, and there were some quirky system clock sync issues. But with subsequent updates, these problems faded away.

Fast forward to now: I'm exploring WSL with Ubuntu 24.04 LTS, and it's been a smooth ride.

---

## 🛠️ Why This Repo?

This repository serves as my personal logbook—a place to document and replicate my WSL setup for future reference. Think of it as my digital breadcrumb trail.

---

## 🚀 Ubuntu 24.04 LTS on WSL

Ubuntu 24.04 LTS, codenamed "Noble Numbat," brings a host of enhancements:

- **Cloud-init support** for streamlined image customization.
- A leaner install size—200MB smaller download.
- Systemd enabled by default, ensuring better compatibility.

These features make Ubuntu 24.04 LTS a robust choice for WSL users. ([canonical.com](https://canonical.com/blog/canonical-releases-ubuntu-24-04-noble-numbat))

---

## 📦 Installation & Setup

To get started with WSL and Ubuntu 24.04 LTS:

1. **Install WSL**:
   ```bash
   wsl --install
   ```
2. **Set Ubuntu 24.04 LTS as your default distribution**:
   ```bash
   wsl --set-default-version 2
   wsl --install -d Ubuntu-24.04
   ```

For a detailed guide, refer to the official [WSL installation documentation](https://learn.microsoft.com/en-us/windows/wsl/install).

---

## 🧑🏽‍💻 Shell Customization – Because Looks Matter Too

Once WSL is installed and running smoothly, it's time to pimp your terminal! Here's how to make your shell not just functional, but fabulous:

### 3. 🌀 Installing ZSH and Setting It as Default

```bash
sudo apt update
sudo apt install zsh -y
chsh -s /bin/zsh
```

Log out and back in—or restart WSL—to start using `zsh`.

---

### 4. ✨ Oh-My-Zsh, Powerlevel10k & Nerd Fonts Setup

Let’s bring the ✨bling✨ to your terminal!

🔗 [Download Nerd Fonts](https://www.nerdfonts.com/font-downloads)  
Extract and install a font of your choice (e.g., `Hack Nerd Font`).

In **Windows Terminal**:
- Go to **Settings → Your WSL profile → Appearance tab**
- Select your installed Nerd Font (e.g., `HackNerdFont`) 🧑🏽‍💻

Then, install Oh-My-Zsh and Powerlevel10k:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

git clone --depth=1 https://github.com/romkatv/powerlevel10k.git \
${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

Update your Zsh config to use the theme:

```bash
vi ~/.zshrc
# Inside .zshrc
ZSH_THEME="powerlevel10k/powerlevel10k"
```

Then run:

```bash
p10k configure
```

Enjoy your shiny new terminal that makes every `ls` feel like an event. 🎉

---

## 🧠 Integrating VS Code with WSL – The Smart Way

Developing in WSL is great, but pairing it with Visual Studio Code takes productivity to the next level. Here's how to set it up:

### 5. 🧩 Install the Remote - WSL Extension

To enable seamless development within WSL, install the **Remote - WSL** extension in VS Code.

- Open VS Code.
- Navigate to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or pressing `Ctrl+Shift+X`.
- Search for `Remote - WSL` and click **Install**.

Once installed, you can open your WSL environment directly in VS Code by opening the Command Palette (`Ctrl+Shift+P`) and selecting `Remote-WSL: New Window`.

---

### 6. 🎨 Customize VS Code Settings for WSL

To enhance your development experience, customize your VS Code settings to align with your WSL environment.

Open your settings (`Ctrl+,`) and switch to the **WSL** context. Then, edit the `settings.json` file to include the following configurations:

```json
{
    "workbench.colorTheme": "Default Dark+",
    "notebook.lineNumbers": "on",
    "files.autoSave": "afterDelay",
    "terminal.integrated.defaultProfile.linux": "zsh",
    "terminal.integrated.fontFamily": "Hack Nerd Font",
    "editor.fontLigatures": false,
    "workbench.iconTheme": "vscode-icons",
    "vsicons.dontShowNewVersionMessage": true,
    "editor.fontFamily": "Hack Nerd Font",
    "workbench.startupEditor": "none"
}
```

These settings ensure that your terminal uses Zsh with the Nerd Font, auto-saves files after a delay, and applies your preferred themes and icons.

---

## 🤝 Contributions & Feedback

While this is a personal project, I'm open to suggestions, improvements, or shared experiences. Feel free to fork, raise issues, or submit pull requests. Let's make WSL setups smoother together!

---

*Happy coding! 🧑‍💻🐧*

---

*Note: For more insights into Ubuntu 24.04 LTS and its features, check out the [official Ubuntu blog](https://ubuntu.com/blog/ubuntu-desktop-24-04-noble-numbat-deep-dive).*
