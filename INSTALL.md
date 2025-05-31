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

You can also open the folder via Keypirinha itself:

1. Launch Keypirinha  
2. Type `Configure`  
3. Select **Keypirinha: Configure** to open the `Keypirinha.ini` file in your default text editor.

## 3. Install the Theme

1. Download the [`keypirinha-dracula-theme.ini`](keypirinha-dracula-theme.ini) file from this repository.
2. Copy it to your user configuration folder (see step 2 above).
3. Open `Keypirinha.ini` and scroll to or create the `[gui]` section.
4. Add or update the following line to reference the theme:

   ```ini
   [gui]
   theme = Dracula
   ```

5. Next, copy the entire contents of `keypirinha-dracula-theme.ini` into the same file (usually just below the `[gui]` section), or keep it as a separate file and copy-paste when needed.

Here’s an example structure in your `Keypirinha.ini`:

```ini
[gui]
theme = Dracula

[theme/Dracula]
; Dracula theme for Keypirinha by Shai (https://github.com/shainave)
; Paste the contents of the keypirinha-dracula-theme.ini file here
; Example:
; ui_font = Segoe UI,10
; ...
```

> 💡 **Section names are case-sensitive**, so `[theme/Dracula]` must match the name in the `theme = Dracula` line exactly.

## 4. Apply the Theme

Save your changes and press `Ctrl+F5` in Keypirinha to reload the configuration. Your Dracula theme should now be active.

## 5. Optional: Customise the Theme

You can customise layout, spacing, fonts, and colours using Keypirinha's theme system. To simplify the process, try the **Keypirinha Theme Builder** by [Fuhrmann](https://github.com/Fuhrmann):

👉 [https://fuhrmann.github.io/keypirinha-theme-builder/](https://fuhrmann.github.io/keypirinha-theme-builder/)

This online tool lets you load, preview, and tweak your theme visually.

## More Information

- [Keypirinha Theming Documentation](https://keypirinha.com/theming.html)
