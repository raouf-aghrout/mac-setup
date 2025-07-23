Mac Setup
=========

Mac setup instructions for development, hopefully turn into a script.

System Settings
---------------

### Control Centre
- Control Centre Modules
  - Set 'Bluetooth' to 'Show in Menu Bar'

### Lock Screen
- Set 'Start Screen Saver when inactive' to 'For 15 minutes'
- Set 'Turn display off on battery when inactive' to 'For 5 minutes'
- Set 'Turn display off on power adapter when inactive' to 'For 5 minutes' 
- Set 'Require password after...' to 'Immediately' 

### Displays
- Select 'More Space'
- Night Shift...
  - Set 'Schedule' to 'Sunset to Sunrise'

### Desktop & Dock
- Remove unused apps
- Slide 'Size' to roughly 25%
- Check 'Minimise windows into application icon'
- Check 'Automatically hide and show the Dock'
- Uncheck 'Show suggested and recent apps in Dock'

### Keyboard
- Slide 'Key Repeat' to 'Fast'
- Slide 'Delay Until Repeat' to 'Short'
- Keyboard Shortcuts...
  - Keyboard
    - Set 'Move focus to next window' to 'command + `'
  - Function Keys
    - Check 'Use F1, F2, etc. keys as standard function keys'

### Trackpad
- Point & Click
  - Check 'Tap to click'
    - Slide 'Tracking speed' to 5
- Scroll & Zoom:
  - Un-check 'Natural scrolling'

Git Settings
------------

1. [Generate a new SSH key and add it to the ssh-agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
    ```shell
    ssh-keygen -t ed25519 -C "your_email@example.com"

    eval "$(ssh-agent -s)"

    touch ~/.ssh/config

    echo "Host github.com\n  AddKeysToAgent yes\n  UseKeychain yes\n  IdentityFile ~/.ssh/id_ed25519" >> ~/.ssh/config

    ssh-add --apple-use-keychain ~/.ssh/id_ed25519
    ```

2. [Add a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
    ```shell
    pbcopy < ~/.ssh/id_ed25519.pub
    ```

3. [Install Homebrew](https://brew.sh/)
    ```shell
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

4. [Install Oh My Zsh](https://ohmyz.sh/#install)
    ```shell
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```

5. Install GPG
    ```shell
    brew install gpg
    ```

6. [Generate a new GPG key](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key)
    ```shell
    gpg --full-generate-key

    gpg --list-secret-keys --keyid-format=long

    gpg --armor --export your_gpg_key_id
    ```

7. [Add the GPG key to your GitHub account](https://docs.github.com/en/authentication/managing-commit-signature-verification/adding-a-gpg-key-to-your-github-account)

8. [Telling Git about your signing key](https://docs.github.com/en/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key)
    ```shell
    git config --global user.signingkey your_gpg_key_id

    git config --global commit.gpgsign true

    git config --global tag.gpgSign true

    if [ -r ~/.zshrc ]; then echo -e '\nexport GPG_TTY=$(tty)' >> ~/.zshrc; else echo -e '\nexport GPG_TTY=$(tty)' >> ~/.zprofile; fi
    ```

9. Run Git setup script
    ```shell
    ./git-setup.sh
    ```

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
