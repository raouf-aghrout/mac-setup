Mac Setup
=========

Mac setup instructions for development, hopefully turn into a script.

System Preferences
------------------

### Control Centre
- Control Centre Modules
	- Bluetooth
		- Set to 'Show in Menu Bar'

### Wallpaper
- Set wallpaper from 'Dynamic Wallpapers'
- Check 'Show as screen saver'

### Lock Screen
- Start Screen Saver when inactive
	- Set 'Start Screen Saver when inactive' to 'Never'
	- Set 'Turn display off on battery when inactive' to 'For 5 minutes'
	- Set 'Turn display off on power adapter when inactive' to 'For 5 minutes' 
	- Set 'Require password...' to 'Immediately' 

### Displays
- Display Settings
        - Select 'More Space'
	- Night Shift...
    		- Set 'Schedule' to 'Sunset to Sunrise'

### Desktop & Dock
- Remove unused apps
- Slide ‘Size' to roughly 25%
- Check ‘Minimise windows into application icon'
- Check ‘Automatically hide and show the Dock’
- Uncheck 'Show suggested and recent apps in Dock'

### Keyboard
- Keyboard:
    	- Slide 'Key Repeat' to 'Fast'
    	- Slide 'Delay Until Repeat' to 'Short'
	- Slide 'Keyboard brightness' to roughly 25%
    	- Touch Bar Settings...
		- Set 'Touch Var shows' to 'F1, F2, etc. Keys'
		- Set 'Press and hold fn key to' to 'Show Expanded Control Strip' 

### Trackpad
- Point & Click
	- Check 'Tap to click’
    	- Slide 'Tracking speed' to 5
- Scroll & Zoom:
    - Un-check ’Natural scrolling'

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
