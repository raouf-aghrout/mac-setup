Mac Setup
=========

Mac setup instructions for development, hopefully turn into a script.

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

### Dock
- Remove unused apps
- Slide ‘Size' to roughly 25%
- Check ‘Automatically hide and show the dock’
- Check ‘Minimise windows into application icon'

### Keyboard
- Keyboard:
    - Set ‘Use all F1, F2, etc. keys as standard function keys’
    - Slide 'Key Repeat' to 'Fast'
    - Slide 'Delay Until Repeat' to 'Short'

### Mouse
- Point & Click
    - Un-check 'Scroll direction: natural'
    - Check ‘Secondary click’
    - Check ‘Smart zoom'
    - Slide ‘Tracking’ to 5
- More Gestures:
    - Check ’Swipe between pages'

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

### Spectacle
- Preferences:
    - Enable only 8 main short cuts
    - Check 'Launch Spectacle at login’
    - Rebind to Ctrl variants

### iTerm
- Keep in dock
- Preferences > Profiles:
    - General:
        - Set 'Working Directory' to 'Reuse previous session's directory'
    - Colors:
        - Set ‘Load Presets…’ to ‘Tango Dark'
    - Terminal:
        - Check 'Unlimited scrollback'

### Oh My Zsh
- Change theme to ‘avit'

### XCode
- Installs developer tools like Git

### Git
- Generate SSH key and setup on GitHub
- Setup config
- Setup aliases

### Brew
- Export Homebrew GitHub API token
- Install recipes:
    - gradle
    - htop
    - java
    - maven
    - node
    - tree
    - unrar

### Node
- Global modules:
    - serverless
    - claudia 

### Google Chrome
- Keep in dock
- Make default browser
- Sign into profile
- Extensions:
    - U Block Origin
    - Ad Block Plus
    - JSON Formatter
    - Momentum

### IntelliJ
- Keep in dock
- On start
    - Select Darcula theme
    - Select Mac OS X 1.5+ key bindings
    - Select default plugins
- Show line numbers
    - Preferences > Editor > General > Appearance:
        - Check 'Show line numbers'
- Remove auto generated file header
    - Preferences > Editor > File and Code Templates > Includes:
        - Delete template under 'File Header'
- Ignore warnings on injected and mock objects
    - Preferences > Editor > Inspections > Java > Declaration redundancy > Unused declaration > Options > Entry points > Configure annotations...
        - Add Autowired / Inject classes
        - Add Mock classes
- Prevent static wildcard imports
    - Preferences > Editor > Code Style > Java > Imports
        - Set 'Class count to use import * ' to 500
        - Set 'Names count to use static import with * ' to 500
- Setup test template
    - Preferences > Editor > Live Templates > Java
        - Create a test live template
- Prevent auto formatting placing annotations on new line
    - Preferences > Editor > Code Style > Java > Wrapping and Braces
        - Set 'Field annotations' to 'Do not wrap'
        - Check 'Do not wrap after single annotation'
- Prevent open tabs remaining on a single row
    - Preferences > Editor > General > Editor Tabs > Tab Appearance
        - Un-check 'Show tabs in single row'

### WebStorm
- Keep in dock
- On Start
    - Select Mac OS X 1.5+ key bindings
    - Select Darcula theme
    - Check 'Enable opening files and projects from the command line'
  
### Caffeine
- Preferences:
    - Check 'Automatically start Caffeine at login'
    - Check 'Activate Caffeine at launch'
    - Un-check 'Show this message when starting Caffeine'

### Spotify
- Keep in dock
- Settings
    - Display Options
        - Enable 'Show unavailable tracks in playlists'
    - Startup and Window Behaviour
        - Set 'Open Spotify automatically after you log into the computer' to 'No' 

### f.lux
### CCleaner
