Mac Setup
=========

Mac setup instructions for development, hopefully turn into a script.

System Preferences
------------------

### Bluetooth
- Check 'Show Bluetooth in menu bar'

### Desktop & Screen Saver
- Desktop:
    - Set background image
- Screen Saver:
    - Uncheck ‘Show screen saver after'

### Displays
- Display Settings:
    - Resolution:
        - Select `Scaled`
	- Select `More Space`
- Night Shift:
    - Set 'Schedule' to 'Sunset to Sunrise'
    - Check 'Turn On Until Sunrise'

### Dock & Menu Bar
- Remove unused apps
- Slide ‘Size' to roughly 25%
- Check ‘Automatically hide and show the Dock’
- Check ‘Minimise windows into application icon'
- Uncheck 'Show recent applications in Dock'

### Keyboard
- Keyboard:
    - Slide 'Key Repeat' to 'Fast'
    - Slide 'Delay Until Repeat' to 'Short'

### Security & Privacy
- General:
    - Change Password...
    - Set ‘Require password’ to ‘immediately'
   
### Trackpad
- Point & Click:
    - Check 'Tap to click’
    - Slide tracking speed to 5
- Scroll & Zoom:
    - Un-check ’Scroll direction: Natural'
- More Gestures:
    - Check ‘App Expose'

### Users & Groups
- Drag and drop profile picture

Brew
----

### XCode
- Installs required developer tools like Git

### Brew
- Install brew
- Install brew formulae:
    - tfswitch
    - zsh
- Install brew casks:
    - caffeine 
    - discord
    - google-chrome
    - iterm2
    - postman
    - slack
    - spectacle
    - spotify
    - webstorm

### Oh My Zsh
- Install Oh My Zsh
    - Change theme to 'avit'

### Git
- Generate SSH key and add to GitHub
- Setup config & aliases

Casks
--------

### Caffeine
- Check 'Automatically start Caffeine at login'
- Check 'Activate Caffeine at launch'
- Un-check 'Show this message when starting Caffeine'

### Google Chrome
- Keep in dock
- Make default browser
- Sign into profiles
- Sync bookmarks
- Setup pinned tabs

### iTerm2
- Keep in dock
- Preferences > Profiles:
    - General:
        - Set 'Working Directory' to 'Reuse previous session's directory'
    - Colors:
        - Set ‘Color Presets…’ to ‘Tango Dark'
    - Terminal:
        - Check 'Unlimited scrollback'

### Postman
- Preferences
    - Themes
        - Select dark theme

### Slack
- Keep in dock
- Preferences
    - Themes
        - Select 'Dark'
        - Colors > Select 'Nocturne'
    - Messages & media
        - Theme > Select 'Compact'

### Spectacle
- Preferences:
    - Enable only 8 main short cuts
    - Check 'Launch Spectacle at login’
    - Rebind to Ctrl variants

### Spotify
- Keep in dock
- Settings
    - Autoplay
        - Disable 'Autoplay similar songs when your music ends'
    - Audio quality
        - Set 'Streaming quality' to 'High'
    - Show Advanced Settings > Startup and window behaviour
        - Set 'Open Spotify automatically after you log into the computer' to 'No'

### Webstorm
- Keep in dock
- On start
    - Select Darcula theme
    - Select default plugins
- Setup test templates
    - Preferences > Editor > Live Templates
- Prevent open tabs remaining on a single row
    - Preferences > Editor > General > Editor Tabs > Appearance
        - Un-check 'Show tabs in on row'
- Plugins:
    - Terraform and HCL
