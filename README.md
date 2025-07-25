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
    - Change theme to 'avit'

5. [Install Oh My Zsh theme - Powerlevel10k](https://github.com/romkatv/powerlevel10k?#oh-my-zsh)
    ```shell
   git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"
    ```
   In `~/.zshrc` set `ZSH_THEME` to "powerlevel10k/powerlevel10k"

6. Install GPG
    ```shell
   brew install gpg
    ```

7. [Generate a new GPG key](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key)
    ```shell
   gpg --full-generate-key

   gpg --list-secret-keys --keyid-format=long

   gpg --armor --export your_gpg_key_id
    ```

8. [Add the GPG key to your GitHub account](https://docs.github.com/en/authentication/managing-commit-signature-verification/adding-a-gpg-key-to-your-github-account)

9. [Telling Git about your signing key](https://docs.github.com/en/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key)
    ```shell
   git config --global user.signingkey your_gpg_key_id

   git config --global commit.gpgsign true

   git config --global tag.gpgSign true

   if [ -r ~/.zshrc ]; then echo -e '\nexport GPG_TTY=$TTY' >> ~/.zshrc; else echo -e '\nexport GPG_TTY=$TTY' >> ~/.zprofile; fi
    ```

10. Run Git setup script
    ```shell
    ./git-setup.sh
    ```

Brew Casks
----------

1. Install Rectangle
    ```shell
    brew install --cask rectangle
    ```
   - Keep only 'Left Half', 'Right Half', 'Top Half', 'Bottom Half', 'Maximise', 'Minimise', 'Next Display' and 
   'Previous Display' shortcuts
   - Settings
     - Check 'Launch on login'

2. Install iTerm2
    ```shell
    brew install --cask iterm2
    ```
    - Keep in dock
    - Settings > Profiles
      - General
        - Set 'Initial directory' to 'Reuse previous session's directory'
      - Colors
        - Set 'Color Preset' to 'Tango Dark'
      - Terminal
        - Check 'Unlimited scrollback'

3. Install IntelliJ
    ```shell
    brew install --cask intellij-idea
    ```
   - Keep in dock
   - Settings > Editor > General > Editor Tabs > Appearance
     - Under 'Show tabs in' check 'Multiples row'

4. Install Google Chrome
    ```shell
    brew install --cask google-chrome
    ```
    - Keep in dock

5. Install Slack:
    ```shell
    brew install --cask slack
    ```
    - Keep in dock

6. Install Spotify:
    ```shell
    brew install --cask spotify
    ```
    - Keep in dock
    - Settings
      - Show Start-up and window behaviour
        - Set 'Open Spotify automatically after you log in to the computer' to 'No'
