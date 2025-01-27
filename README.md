# Minimalist Firefox UI Theme

This project customizes the Firefox UI using a `userChrome.css` file to achieve a minimalist aesthetic inspired by browsers like QuteBrowser. The theme is built around the Gruvbox color palette and focuses on simplicity, efficiency, and a clean user interface. The sizing of elements is optimized for a 15-in 2023 macbook, and may need tweaking.

## Features

### 1. **Minimal Window Decorations**
   - Removes unnecessary window decorations like the title bar and button box to maximize usable screen space.

### 2. **Streamlined Toolbar**
   - Simplifies the toolbar by hiding redundant buttons such as:
     - Back/Forward
     - Downloads
     - Bookmarks Menu
     - Sidebar Toggle
   - Customizes the toolbar’s appearance with consistent dimensions and Gruvbox styling.

### 3. **Optimized Tabs**
   - Ensures tabs are compact, with no extra padding or borders.
   - Highlights the active tab with a subtle Gruvbox background.
   - Removes close buttons from tabs for a cleaner look.

### 4. **Auto-Hiding URL Bar**
   - The URL bar remains hidden by default, becoming visible only when focused (with the cmd+l command)
   - Smooth animations for showing and hiding elements.

### 5. **Custom Context Menus**
   - Restyled context menus to match the Gruvbox theme.
   - Clean and responsive hover states for menu items.

### 6. **Other Enhancements**
   - Removes scrollbars for a distraction-free experience.
   - Simplifies the status bar and tooltips.

## Installation

1. **Enable userChrome.css**
   - Open Firefox and go to `about:config`.
   - Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and set it to `true`.

2. **Locate Your Profile Folder**
   - In Firefox, go to `about:support` and locate the “Profile Folder”.
   - Click “Open Folder” to access your profile directory.

3. **Add the CSS File**
   - Create a `chrome` folder in your profile directory if it doesn’t already exist.
   - Place the `userChrome.css` file into the `chrome` folder.

4. **Restart Firefox**
   - Restart Firefox to apply the changes.

## Customization

- The theme uses CSS variables for easy customization. Adjust colors, dimensions, and other settings in the `:root` section of the CSS file.
  ```css
  :root {
      --gruvbox-bg: #282828;
      --gruvbox-fg: #ebdbb2;
      --icon-size: 16px;
      --tab-height: 37px;
  }
  ```

## Notes

- Some elements are intentionally hidden to align with the minimalist philosophy. If needed, you can uncomment or modify specific sections in the CSS file.
- Test your changes by reloading Firefox to ensure they are applied correctly.

## Acknowledgments

This theme draws inspiration from QuteBrowser and the minimalist Firefox customizations by [github/dook97](https://github.com/dook97).

## Feedback

If you encounter issues or have suggestions for improvement, feel free to contribute or reach out!

