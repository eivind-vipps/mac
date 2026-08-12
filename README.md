# Configuration management for work MacBook

MacBook Pro 14" 2021, M1 Pro, 32GB.

Install with English language and Norwegian region. Remove Norwegian keyboard.
Do not login to iCloud.

## Setup

- Install build dependencies for Homebrew:

  ```sh
  xcode-select --install
  ```

- Install Homebrew:

  ```sh
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```

- Provide secrets:

  ```sh
  cat <<EOF >secrets.sh
  GIT_NAME='Your Name'
  GIT_EMAIL='your@name.tld'
  EOF
  ```

- Provision the system:

  ```sh
  ./run.sh
  ```

## GUI Settings

### System settings

- Apple Account
  - Sign in
  - iCloud
    - Photos
      - Sync this Mac: disable
- Bluetooth
  - Air Pods Pro
    - Options
      - [ ] Connect to This Mac: When Last Connected to This Mac
- Appearance
  - Liquid Glass: solid
- Desktop & Dock
  - Desktop & State Manager
    - [ ] Show Items: disable On Desktop
  - Widgets
    - [ ] Show Widgets: disable On Desktop
- Menu Bar
  - [ ] Screen Mirroring: Always Show in Menu Bar
- Wallpaper
  - [ ] Color: orange
- Sound
  - [ ] Play sound on startup: disable
  - [ ] Play user interface sound effects: disable
- Touch ID & Password
  - [ ] Add Fingerprint
- Keyboard
  - Keyboard shortcuts
    - Modifier keys (select both internal and external keyboards)
      - [ ] Caps Lock: Escape

### Mission Control

- [ ] Add one more space.

### Safari

- Settings
  - General
    - [ ] Safari opens with: all non-private windows from last session
  - Advanced
    - [ ] Smart search field: show full website address
    - [ ] Show features for web developers: enable
- View
  - [ ] Show Status Bar

### Messags

- Settigns
  - iMessage
    - Apple Acount: Sign Out

### KeepingYouAwake

- Settings
  - General
    - [ ] Start at login: enable
  - Activation Duration:
    - [ ] Add: 7 hours
