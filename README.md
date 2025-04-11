# Starship Prompt: Powerlevel10k Lookalike ✨🚀

This repository contains a Starship configuration (`starship.toml`) designed to mimic the popular [Powerlevel10k](https://github.com/romkatv/powerlevel10k) Zsh theme. It leverages Starship's flexibility to recreate a similar aesthetic and information display for any shell compatible with Starship.

This configuration was primarily tested with **iTerm2** on macOS, but should work on other modern terminal emulators that support Nerd Fonts.

## 📸 Preview

![Screenshot of the Starship prompt in action](![image](https://github.com/user-attachments/assets/7ca9a33a-acb2-4b55-8497-f4d2e95494c4)
)

## ✨ Features

*   **Powerline Style:** Uses Powerline symbols (``, ``, ``, ``) for segment separation, mimicking the p10k look.
*   **Git Integration:** Displays current Git branch, status icons (like `✗` for errors), and counts for added/deleted lines (`git_metrics`). Uses `` symbol for branch.
*   **Directory Display:** Shows the current path styled within segments.
*   **Python Virtualenv:** Clearly indicates the active Python virtual environment using segments.
*   **Command Status:** Shows an error symbol (`✗`) on failure.
*   **Minimalist Right Prompt:** Configured to potentially show Python info on the right (can be customized further).

## Prerequisites

1.  **Terminal Emulator:** A modern terminal emulator is needed. This config is optimized for **iTerm2**, but others like Kitty, Alacritty, WezTerm, or Windows Terminal should work.
2.  **Nerd Font:** **This is essential!** The configuration heavily relies on glyphs (icons and Powerline symbols) provided by Nerd Fonts. You **must** install a Nerd Font and configure your terminal emulator (e.g., iTerm2 -> Profiles -> Text -> Font) to use it.
    *   **Download Nerd Fonts:** [https://www.nerdfonts.com/](https://www.nerdfonts.com/) (Popular choices: FiraCode Nerd Font, MesloLGS NF, JetBrainsMono Nerd Font)
3.  **Starship:** You need Starship installed and configured in your shell.

## 🚀 Installation Guide

Follow these steps to install Starship and apply this configuration:

**Step 1: Install Starship**

If you haven't already, install Starship using the official instructions for your operating system and shell:
[https://starship.rs/guide/#installation](https://starship.rs/guide/#installation)

*   Make sure to follow the instructions to add the Starship initialization line to your shell's configuration file (e.g., `.zshrc`, `.bashrc`, `.config/fish/config.fish`).

**Step 2: Install and Configure a Nerd Font**

*   Download and install a Nerd Font from [Nerd Fonts](https://www.nerdfonts.com/). Follow their instructions for your OS.
*   Configure your terminal emulator to use the installed Nerd Font.
    *   *Example for iTerm2:* Go to `Preferences` > `Profiles` > `(Your Profile)` > `Text` > `Font` section, and select your installed Nerd Font. Ensure "Use ligatures" is checked if your font supports them.

**Step 3: Apply This Configuration**

1.  **Backup (Optional but Recommended):** If you have an existing Starship config, back it up:
    ```bash
    mv ~/.config/starship.toml ~/.config/starship.toml.bak
    ```
    *(If the directory `~/.config` doesn't exist, the next command will create it)*

2.  **Download this configuration file:** Choose one method:

    *   **Using `curl`:**
        ```bash
        mkdir -p ~/.config && curl -o ~/.config/starship.toml https://raw.githubusercontent.com/[Your GitHub Username]/[Your Repository Name]/main/starship.toml
        ```
        *(Replace `[Your GitHub Username]` and `[Your Repository Name]`)*

    *   **Using `wget`:**
        ```bash
        mkdir -p ~/.config && wget -O ~/.config/starship.toml https://raw.githubusercontent.com/[Your GitHub Username]/[Your Repository Name]/main/starship.toml
        ```
        *(Replace `[Your GitHub Username]` and `[Your Repository Name]`)*

    *   **Manual Download:** Download the `starship.toml` file from this repository and save it to `~/.config/starship.toml`.

**Step 4: Reload Your Shell**

Close and reopen your terminal window, or source your shell's configuration file (e.g., `source ~/.zshrc`, `source ~/.bashrc`) for the changes to take effect.

You should now see the Powerlevel10k-like prompt!

## 🎨 Customization

This configuration serves as a starting point. You can customize it further by editing the `~/.config/starship.toml` file. Refer to the official Starship documentation for all available options:

*   **Configuration:** [https://starship.rs/config/](https://starship.rs/config/)
*   **Modules:** [https://starship.rs/config/#prompt](https://starship.rs/config/#prompt) (See sidebar for specific modules like `[git_branch]`, `[directory]`, etc.)

## 📄 License

This configuration is shared under the [MIT License](LICENSE).
