# Puush in Linux

Takes screenshots and uploads them to puush using the puush API and copies the link to clipboard. Recommended for set up with keyboard shortcuts
<br>Supports both GNOME and KDE desktop environments. Utilises **gnome-screenshot** or **spectacle** for taking screenshots, **zenity** or **kdialog** for file uploads.

## Instructions

- Clone or download the repo
- In file "puush" add your puush API key to PUUSH_API_KEY
  - (You can find your API key at http://puush.me/account/settings)
- Make it executable using **chmod +x puush**
- Place this file wherever you want (recommended: /usr/local/bin)
- Set up keyboard shortcuts within linux
  - (in Ubuntu it's system settings > keyboard > keyboard shortcuts > custom shortcuts)
  - Log out for the changes to take place
  - Here's what it looks like for mine: ![Puush keyboard setup](http://puu.sh/cOyVz/8dcb1cd498.png)

### Commands

```bash
puush -a		# puush desktop
puush -b		# area puush
puush -c		# puush window
puush -d		# file upload
puush -e		# puush clipboard

puush -h  	  # help
```

## Dependencies

### GNOME Desktop Environment

- gnome-screenshot
- zenity
- curl
- xclip
- notify-send

### KDE Desktop Environment

- spectacle
- kdialog (optional, falls back to zenity)
- curl
- xclip
- notify-send

### Alternatives

- puush in command line https://github.com/blha303/puush-linux
- puush using keyboard https://github.com/sgoo/puush-linux
