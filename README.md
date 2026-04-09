Getting as close to GitHub's Primer Theme as possible.

After each update, you may need to re-select your editor theme by going to: **Settings -> Editor -> Color Scheme -> Scheme dropdown**

Installation instructions:
1. Install plugin from JetBrains Marketplace
2. To enable the editor theme, navigate to **Settings -> Editor -> Color Scheme -> Scheme dropdown**
3. Dark theme is applied upon installation by default. To change to Dimmed: navigate to **Settings -> Appearance -> Theme** dropdown
4. Restart IDE for good measure
 
[Intellij Plugin Repository](https://plugins.jetbrains.com/plugin/19291-github-dark) | [Report an issue](https://github.com/toby-j/Intellij_GitHub_Dark_Theme/issues)  

![Screenshot](screenshots/7-small.png)

![Screenshot](screenshots/8-small.png)
 
# Colour Palette

Colours sourced from [GitHub's Primer design system](https://github.com/primer/github-vscode-theme), matching the GitHub Codespaces editor theme.

## Dark
| Role | Colour | Token |
|------|--------|-------|
| Keywords / Operators | ![#FF7B72](https://placehold.co/15x15/FF7B72/FF7B72.png) `#FF7B72` | Red |
| Functions | ![#D2A8FF](https://placehold.co/15x15/D2A8FF/D2A8FF.png) `#D2A8FF` | Purple |
| Variables / Entity names | ![#FFA657](https://placehold.co/15x15/FFA657/FFA657.png) `#FFA657` | Orange |
| Foreground text | ![#E6EDF3](https://placehold.co/15x15/E6EDF3/E6EDF3.png) `#E6EDF3` | |
| Strings / Regex | ![#A5D6FF](https://placehold.co/15x15/A5D6FF/A5D6FF.png) `#A5D6FF` | Blue light |
| Constants / Numbers / Support | ![#79C0FF](https://placehold.co/15x15/79C0FF/79C0FF.png) `#79C0FF` | Blue |
| HTML tags / JSON keys | ![#7EE787](https://placehold.co/15x15/7EE787/7EE787.png) `#7EE787` | Green |
| Constants (special) | ![#F692CE](https://placehold.co/15x15/F692CE/F692CE.png) `#F692CE` | Pink |
| Comments | ![#8B949E](https://placehold.co/15x15/8B949E/8B949E.png) `#8B949E` | Grey |

## Dimmed
| Role | Colour | Token |
|------|--------|-------|
| Keywords / Operators | ![#F47067](https://placehold.co/15x15/F47067/F47067.png) `#F47067` | Red |
| Functions | ![#DCBDFB](https://placehold.co/15x15/DCBDFB/DCBDFB.png) `#DCBDFB` | Purple |
| Variables / Entity names | ![#F69D50](https://placehold.co/15x15/F69D50/F69D50.png) `#F69D50` | Orange |
| Foreground text | ![#ADBAC7](https://placehold.co/15x15/ADBAC7/ADBAC7.png) `#C9D1D9FF` | |
| Strings / Regex | ![#96D0FF](https://placehold.co/15x15/96D0FF/96D0FF.png) `#96D0FF` | Blue light |
| Constants / Numbers / Support | ![#6CB6FF](https://placehold.co/15x15/6CB6FF/6CB6FF.png) `#6CB6FF` | Blue |
| HTML tags / JSON keys | ![#8DDB8C](https://placehold.co/15x15/8DDB8C/8DDB8C.png) `#8DDB8C` | Green |
| Constants (special) | ![#F692CE](https://placehold.co/15x15/F692CE/F692CE.png) `#F692CE` | Pink |
| Comments | ![#768390](https://placehold.co/15x15/768390/768390.png) `#768390` | Grey |

# Contributions

There's plenty more work to do on this plugin, so if you'd like to lend a hand here's how you can.

This is made using DevKit, not Gradle. ([This project might have to be migrated to eventually...](https://plugins.jetbrains.com/docs/intellij/migrating-plugin-devkit-to-gradle.html))

This is the easiest way I found to work on it. For further reading: [here's the official guide](https://plugins.jetbrains.com/docs/intellij/themes-getting-started.html?from=DevkitOpenThemeReference#gradle-based-theme-project)

## Prerequisites 
1. Clone repository on Intellij IDEA Ultimate and open it.
2. Install the plugin "Plugin DevKit" by Intellij
3. Install the latest version of this plugin from the Intellij Marketplace
## Editing
Inside of **resources/themes/** you'll find the `.xml` for the code window and `.json` for everything else (dialog boxes, terminal etc...) for each of the themes.

Working with them requires slightly different approaches.

### .XML
1. Navigate to **Editor -> Color Scheme -> General**
2. Select the theme you wish to edit
3. Make the changes using the GUI.
4. Once you've finished with your edits, export your edited color scheme as an `.icls` (Small cog on the **Editor -> Color Scheme -> General** dialog)
5. With this repository open on Intellij IDEA Ultimate, replace the old `.icls` file with the new one you just exported.

### .JSON
I found the [LaF Defaults tool](https://plugins.jetbrains.com/docs/intellij/internal-ui-laf-defaults.html) useful for editing this.
You can edit the `.json` file and test it out by pressing the play button at the top of the file once you have it open.

## Testing
1. Right click the project window and select "Prepare Plugin Module 'intellijgithub_dark_theme' for Deployment" and save somewhere.
2. You can now load this exported plugin file into any of the Intellij IDEs by navigating to **Settings -> Plugins** pressing the settings cog and selecting "Install Plugin from Disk".

Once you've finished testing and happy with your edits, please feel free to open a pull request! 🚀
