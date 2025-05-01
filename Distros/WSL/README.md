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

## 🤝 Contributions & Feedback

While this is a personal project, I'm open to suggestions, improvements, or shared experiences. Feel free to fork, raise issues, or submit pull requests. Let's make WSL setups smoother together!

---

*Happy coding! 🧑‍💻🐧*

---

*Note: For more insights into Ubuntu 24.04 LTS and its features, check out the [official Ubuntu blog](https://ubuntu.com/blog/ubuntu-desktop-24-04-noble-numbat-deep-dive).*
