# Install

## 1. Download Keypirinha

If you haven't already, download Keypirinha from [keypirinha.com](https://keypirinha.com/).

## 2. Locate Your User Configuration Folder

Keypirinha stores user configuration files in different locations depending on how it's installed:

- **Portable version**:  
  ```
  Keypirinha\portable\Profile\User\
  ```

- **Installed version**:  
  ```
  %APPDATA%\Keypirinha\Profile\User\
  ```

You can also open the configuration file via Keypirinha itself:

1. Launch Keypirinha  
2. Type `Configure`  
3. Select `Keypirinha: Configure` to open the `Keypirinha.ini` file in your default text editor.

## 3. Install the Theme

1. Download the [`keypirinha-dracula-theme.ini`](keypirinha-dracula-theme.ini) file from this repository.
2. Open `Keypirinha.ini` and update or create the following line in the `[gui]` section to reference the theme:

   ```ini
   [gui]
   theme = Dracula
   ```

5. Next, copy the entire content of `keypirinha-dracula-theme.ini` into the same file (usually just below the `[gui]` section).

Here’s an example structure in your `Keypirinha.ini`:

```ini
[gui]
theme = Dracula

[theme/Dracula]
; Dracula theme for Keypirinha by Shai (https://github.com/shainave)
; Paste the contents of the keypirinha-dracula-theme.ini file here
; ...
```

> [!Note]
> Section names are case-sensitive**, so `[theme/Dracula]` must match the name in the `theme = Dracula` line exactly.

## 4. Apply the Theme

Save your changes and press `Ctrl+F5` in Keypirinha to reload the configuration. Your Dracula theme should now be active.

## 5. Optional: Customise the Theme

This theme uses the **JetBrains Mono** font by default, with sensible fallback fonts. You can download JetBrains Mono (Nerd Font patched) from [this release link](https://github.com/ryanoasis/nerd-fonts/releases/download/v3.4.0/JetBrainsMono.zip).

You can further customise layout, spacing, fonts, and colours by editing the theme values. To simplify the process, try the [Keypirinha Theme Builder](https://fuhrmann.github.io/keypirinha-theme-builder/) by [Fuhrmann](https://github.com/Fuhrmann), which lets you load, preview, and tweak your theme visually.


## More Information

- [Keypirinha Theming Documentation](https://keypirinha.com/theming.html)
