Mac Setup
=========

Mac setup instructions for development, hopefully turn into a script.

To Do:
------

- Brew all the things
- Add IntelliJ plugins

System Preferences
------------------

### Bluetooth
- Pair mouse and rename
- Pair keyboard and rename

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

### Keyboard
- Keyboard:
    - Slide 'Key Repeat' to 'Fast'
    - Slide 'Delay Until Repeat' to 'Short'
- Shortcuts:
    - Functions keys:
        - WebStorm
        - IntelliJ IDEA CE
- Keyboard:
    - Customize Control Strip:
        - Screen Lock

### Mouse
- Point & Click
    - Un-check 'Scroll direction: natural'
    - Check ‘Secondary click’
    - Check ‘Smart zoom'
    - Slide ‘Tracking’ to 5
- More Gestures:
    - Check ’Swipe between pages'
    
### Network
- Advanced...
    - DNS
        - Add DNS servers 8.8.8.8 & 8.8.4.4
        - Remove others

### Security & Privacy
- General:
    - Change Password...
    - Set ‘Require password’ to ‘immediately'

### Trackpad
- Point & Click:
    - Check 'Tap to click’
    - Slide tracking speed to 5
- Scroll & Zoom:
    - Un-check ’Scroll direction: natural
- More Gestures:
    - Check ‘App Expose'

### Users & Groups
- Drag and drop profile picture

Software
--------

### Google Chrome
- Keep in dock
- Make default browser
- Sign into profile
- Extensions:
    - U Block
    - JSON Formatter
    - Momentum
    - 1Password
    - React Developer Tools

### Spectacle
- Preferences:
    - Enable only 8 main short cuts
    - Check 'Launch Spectacle at login’
    - Rebind to Ctrl variants

### iTerm2
- Keep in dock
- Preferences > Profiles:
    - General:
        - Set 'Working Directory' to 'Reuse previous session's directory'
    - Colors:
        - Set ‘Color Presets…’ to ‘Tango Dark'
    - Terminal:
        - Check 'Unlimited scrollback'

### XCode
- Installs developer tools like Git

### Oh My Zsh
- Change theme to ‘avit'

### Git
- Generate SSH key and setup on GitHub
- Setup config
- Setup aliases

### Brew
- Install casks:
    - java8
    - cyberduck
    - fly
    - avibrazil-rdm
    - caffeine
    - docker
    - tunnelblick
    - postman
- Install recipes:
    - gradle
    - htop
    - node
    - tree
    - unrar
    - awscli
    - aws-elasticbeanstalk
    - docker
    - tfenv
    - ccat

### Caffeine
- Check 'Automatically start Caffeine at login'
- Check 'Activate Caffeine at launch'
- Set Default duration 'Indefinitely'

### Node
- Global modules:
    - serverless
    - claudia 

### IntelliJ
- Keep in dock
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

### Postman
- Keep in dock

### 1Password
### CCleaner
