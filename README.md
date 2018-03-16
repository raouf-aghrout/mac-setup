Mac Setup
=========

Mac setup instructions for development, hopefully turn into a script.

To Do:
------

- Brew all the things
- Add IntelliJ plugins

System Preferences
------------------

### Trackpad
- Point & Click:
    - Check 'Tap to click’
    - Slide tracking speed to 5
- Scroll & Zoom:
    - Un-check ’Scroll direction: natural
- More Gestures:
    - Check ‘App Expose'

### Keyboard
- Keyboard:
    - Slide 'Key Repeat' to 'Fast'
    - Slide 'Delay Until Repeat' to 'Short'
    - Customize Control Strip:
        - Screen Lock

### Desktop & Screen Saver
- Desktop:
    - Set background image
- Screen Saver:
    - Set ‘Start after’ to 'Never'

### Displays
- Display:
    - Slide display resolution to scaled for ‘More Space’
- Night Shift:
    - Set 'Schedule' to 'Sunset to Sunrise'
    - Check 'Turn On Until Sunrise'

### Dock
- Remove unused apps
- Slide ‘Size' to roughly 25%
- Check ‘Automatically hide and show the dock’
- Check ‘Minimise windows into application icon'
    
### Network
- Advanced...
    - DNS
        - Add DNS servers 8.8.8.8 & 8.8.4.4

### Security & Privacy
- General:
    - Change Password...
    - Set ‘Require password’ to ‘immediately'

### Users & Groups
- Drag and drop profile picture

Brew
----

### XCode
- Installs required developer tools like Git

### Brew
- Install recipes:
    - awscli
    - ccat
    - gradle
    - htop
    - maven
    - node
    - tree
    - unrar
- Install brew cask
- Install casks:
    - iterm2
    - google-chrome
    - java8
    - caffeine

Software
--------

### iTerm2
- Keep in dock
- Preferences > Profiles:
    - General:
        - Set 'Working Directory' to 'Reuse previous session's directory'
    - Colors:
        - Set ‘Color Presets…’ to ‘Tango Dark'
    - Terminal:
        - Check 'Unlimited scrollback'

### Oh My Zsh
- Change theme to ‘avit'

### Google Chrome
- Keep in dock
- Make default browser
- Sign into profiles
- Sync bookmarks
- Setup pinned tabs
- Install extensions:
    - LastPass
    - U Block
    - JSON Formatter
    - Momentum
    - React Developer Tools

### Spectacle
- Preferences:
    - Enable only 8 main short cuts
    - Check 'Launch Spectacle at login’
    - Rebind to Ctrl variants

### Git
- Generate SSH key and setup on GitHub
- Setup config
- Setup aliases

### Caffeine
- Check 'Automatically start Caffeine at login'
- Check 'Activate Caffeine at launch'
- Set Default duration 'Indefinitely' 

### IntelliJ
- Keep in dock
- Setup System Preferences > Keyboard > Shortcuts > Functions keys
- On start
    - Select Darcula theme
    - Select Mac OS X 1.5+ key bindings
    - Select default plugins
- Ignore warnings on injected and mock objects
    - Preferences > Editor > Inspections > Java > Declaration redundancy > Unused declaration > Options > Entry points > Annotations...
        - Add Autowired, Inject, Mock etc. to 'Mark field as implicilty written if annotated by'
- Prevent static wildcard imports
    - Preferences > Editor > Code Style > Java > Imports
        - Set 'Class count to use import * ' to 500
        - Set 'Names count to use static import with * ' to 500
- Setup test template
    - Preferences > Editor > Live Templates > Java
        - Create a test live template
- Prevent open tabs remaining on a single row
    - Preferences > Editor > General > Editor Tabs > Tab Appearance
        - Un-check 'Show tabs in single row'`

### WebStorm
- Keep in dock
- Setup System Preferences > Keyboard > Shortcuts > Functions keys
- On Start
    - Select Darcula theme
    - Select Mac OS X 1.5+ key bindings
    - Check 'Enable opening files and projects from the command line'
- Apply JavaScript code formatting options
    - Preferences > Editor > CodeStyle > JavaScript
        - Set 'Tab size' to 2
        - Set 'Indent' to 2
        - Set 'Continuation indent' to 2
- Plugins:
    - .ignore
    - BashSupport
    - HashiCorp Terraform / HCL language support
    - Markdown support

### Spotify
- Keep in dock
- Settings
    - Music Quality
        - Enable 'High quality streaming'
    - Display Options
        - Enable 'Show unavailable tracks in playlists'
    - Startup and Window Behaviour
        - Set 'Open Spotify automatically after you log into the computer' to 'No' 

### Slack
- Keep in dock

### CCleaner
