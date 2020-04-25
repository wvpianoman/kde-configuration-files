# KDE config file paths

---
### Configurations that cannot be changed from GUI
  * hide title bar when windows are maximized
     * `kwriteconfig5 --file $HOME/.config/kwinrc --group Windows --key BorderlessMaximizedWindows true`
  * [Delete all (i hope) config files](https://github.com/shalva97/kde-configuration-files/blob/master/delete-kde-configuration-files.fish)

#### Panel
   * `.config/plasma-org.kde.plasma.desktop-appletsrc`

#### Appearance
   * Look and Feel
      * `.config/kcminputrc`
      * `.config/kdeglobals`
      * `.config/kscreenlockerrc`
      * `.config/ksplashrc`
      * `.config/kwinrc`
      * `.config/plasmarc`
   * Workspace Theme
      * Splash Screen
         * `.config/ksplashrc`
      * Plasma Theme
         * `.config/plasmarc`
      * Cursors
         * `.config/kcminputrc`
   * Colors
       * `.config/kdeglobals`
       * `.config/Trolltech.conf`
   * Fonts
      * Fonts
         * `.config/kdeglobals`
         * `.config/kcmfonts`
   * Icons
      * `.config/kdeglobals` [Icons]
   * Application Style
      * `.config/kdeglobals`
      * Window Decorations
         * `.config/kwinrc`
#### Workspace
   * Desktop behavior
      * Workspace
         * `.config/plasmarc`
      * Desktop behavior
         * [Screen Edges](#screen-edges)
            * `.config/kwinrc`
   * Window Management
      * Window  behavior
         * `.config/kwnirc`
      * Window Rules
         * `.config/kwinrulesrc`
   * Shortcuts
      * Custom Shortcuts
         * `.config/khotkeys`
      * Global Shortcuts
         * `.config/kglobalshortcutsrc`
   * Startup and Shutdown
      * Background Services
          * `.config/kded5rc`
       * Desktop Session
          * `.config/ksmserverrc`
   * Search
      * Plasma Search
         * `.config/krunnerrc`
      * File Search
         * `.config/baloofilerc`
#### Personalization
   * Account Details
   * Notifications
      * `.config/plasmanotifyrc`
   * Regional Settings
      * Formats
         * `.config/plasma-localerc`
      * Date & Time
         * `.config/ktimezonedrc`
   * Accessibility
      * `.config/kaccessrc`
   * Applications
      * Default Applications
         * `.config/kdeglobals`
#### Network
   * Connections
      * `/etc/NetworkManager/system-connections`
   * Settings
   * Bluetooth
      * `.config/bluedevilglobalrc`
#### Hardware
   * Input Devices
      * Keyboard
         * Hardware
            * `.config/kcminputrc`
         * layout
            * TODO
         * Advanced
            * `.config/kxkbrc`
   * Display and Monitor
      * Gamma
         * `.config/kgammarc`
   * Multimedia
   * Power Management
      * Energy Saving
         * `.config/powermanagementprofilesrc`
   * KDE Connect
      * `.config/kdeconnect`
   * Removable Storage

## Screen Edges
### Active Screen Corners and Edges
Corners are numbered like this:

```
7 - 8 - 3
6 -   - 2
5 - 4 - 1
```

actions are defined in [ElectricBorders] and animations are in other groups, probably in \[effect-\*] and \[TabBox\]. To Disable them run these [commands](https://github.com/shalva97/kde-configuration-files/blob/de8f766da881fd6de828c3ecbbeb48d8bc25fd79/setupKDE.fish#L10-L24)

### Window Management
[Windows]

Maximize windows by dragging them to the top of the screen, boolean value

ElectricBorderMaximize: Boolean

Tiling

ElectricBorderTiling: Boolean
