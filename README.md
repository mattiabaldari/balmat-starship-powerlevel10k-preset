# Starship Prompt: Powerlevel10k Lookalike ✨🚀

This repository contains a Starship configuration (`starship.toml`) designed to mimic the popular [Powerlevel10k](https://github.com/romkatv/powerlevel10k) Zsh theme. It leverages Starship's flexibility to recreate a similar aesthetic and information display for any shell compatible with Starship.

This configuration was primarily tested with **iTerm2** on macOS, but should work on other modern terminal emulators that support Nerd Fonts.

## 📸 Preview

![Screenshot of the Starship prompt in action](https://github.com/user-attachments/assets/985f19dd-4e7f-4553-8955-b3772ad28c67)

## Prerequisites

1.  **Terminal Emulator:** A modern terminal emulator is needed. This config is optimized for **iTerm2**, but others like Kitty, Alacritty, WezTerm, or Windows Terminal should work.
2.  **Starship:** You need Starship installed and configured in your shell.

## 🚀 Installation Guide

Follow these steps to install Starship and apply this configuration:

**Step 1: Install Starship**

If you haven't already, install Starship using the official instructions for your operating system and shell:
[https://starship.rs/guide/#installation](https://starship.rs/guide/#installation)

*   Make sure to follow the instructions to add the Starship initialization line to your shell's configuration file (e.g., `.zshrc`, `.bashrc`, `.config/fish/config.fish`).

**Step 2: Apply This Configuration**

1.  **Download this configuration file:** Choose one method:

    *   **Using `curl`:**
        ```bash
        mkdir -p ~/.config && curl -o ~/.config/starship.toml https://raw.githubusercontent.com/mattiabaldari/balmat-starship-powerlevel10k-preset/main/starship.toml
        ```

    *   **Using `wget`:**
        ```bash
        mkdir -p ~/.config && wget -O ~/.config/starship.toml https://raw.githubusercontent.com/mattiabaldari/balmat-starship-powerlevel10k-preset/main/starship.toml
        ```

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
