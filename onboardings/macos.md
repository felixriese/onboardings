# Onboarding on macOS

In the following, we give an overview of onboarding on a new MacBook or iMac.

## Software

### Most Important

* [OmniFocus](https://www.omnigroup.com/omnifocus) for task management and *getting things done*
* [Mindnode](https://mindnode.com) for mindmapping
* Apple TimeMachine for backups, [Carbon Copy Cloner](https://bombich.com/de) for bootable backups, [Arq](https://www.arqbackup.com) as offsite backup solution with Dropbox
* [1Password](https://1password.com) for saving passwords and account information
* [Bear](http://www.bear-writer.com) for notes in Markdown and [Typora](https://typora.io) as standalone Markdown reader
* Apple Safari as browser, sometimes [Firefox](https://www.mozilla.org/de/firefox/new/) or [Chrome](https://www.google.com/chrome/browser/desktop/index.html)
  * Useful Safari addons: [uBlock](https://www.ublock.org)
  * Useful Firefox/Chrome addons: [HTTPS Everywhere](https://www.eff.org/https-everywhere)
* Cloud: [Dropbox](https://www.dropbox.com)
* Apple Keynote and [PowerPoint 2019](https://products.office.com/de-de/powerpoint) for presentations (sometimes also LaTeX, see below)
* [Word 2019](https://products.office.com/de-de/word) for documents
* [Excel 2019](https://products.office.com/de-de/excel) and Apple Numbers for tables
* Apple Mail for E-Mails
* [Spotify](https://www.spotify.com) (Premium) for music
* [Hazel](https://www.noodlesoft.com) for (document) automation

### For Coding and Scientific Work

* Build-in zsh terminal
* [Homebrew](https://brew.sh/index_de.html)
* [OmniGraffle](https://www.omnigroup.com/omnigraffle/) for flowcharts
* [Textmate](http://macromates.com) and [VSCode](https://code.visualstudio.com) as text editor (definitively not perfect)
* LaTeX:
  * [Texpad](https://www.texpad.com) & [MacTex](http://www.tug.org/mactex/)
  * Online: Overleaf
* [Yummy FTP](http://www.yummysoftware.com)
* [Tunnelblick](https://tunnelblick.net) for VPN tunnels
* [Slack](https://slack.com) for team collaboration
* [Trello](https://trello.com) for Kanban boards in teams
* [Skype](https://www.skype.com/de/download-skype/skype-for-mac/) for video calls
* [Teamviewer](https://www.teamviewer.com/) for controlling the measurement computers from remote
* [QGIS](http://www.qgis.org/) as geographic information system

### Other Tools

* [Pocket](https://getpocket.com/mac/?a=mac) for offline articles and [Reeder](http://reederapp.com/mac/) for RSS feeds
* [PDF Expert](https://pdfexpert.com) for PDF annotations etc.
* [OmniOutliner](https://www.omnigroup.com/omnioutliner) for outlines of papers, workshops etc.
* Apple Photos
* [Tripmode](https://www.tripmode.ch) as blocker for outgoing connections while tethering via iPhone
* [Magnet](https://itunes.apple.com/de/app/magnet/id441258766?mt=12) for window management
* [Bartender](https://www.macbartender.com) for a organizing my menu bar
* [CleanMyMac](https://macpaw.com/cleanmymac) for easily cleaning, optimizing and maintaining

## macOS Settings

* Deactivate the window animations with  `defaults write NSGlobalDomain NSAutomaticWindowAnimationsEnabled -bool NO` in the terminal
* Activate text selection in quick look with `defaults write com.apple.finder QLEnableTextSelection -bool TRUE` in the terminal
* Show battery percentage in `System Preferences > Energy Saver`
* Enable  `System Preferences > Trackpad > Tap to click`
* Enable `System Preferences > Accessibility > Mouse & Trackpad > Trackpad Options > Enable dragging with 3 fingers`
* Disable the warning when changing a file extension: `defaults write com.apple.finder FXEnableExtensionChangeWarning -bool false`
* Hide the hard drive on the Desktop: `Finder > Preferences > General > Show these items on the desktop`
* My iCloud settings:
  * Activate iCloud Drive
    * Deactivate Folder "Desktop" & Documents
    * Deactivate "Optimize Mac storage"
  * Activate "Use Find My Mac"
* Save as PDF shortcut: If you want to save a file as PDF, use the following shortcut. Go to `System Preferences > Keyboard > Shortcuts > App shortcuts` and create a new shortcut for *all apps* as "Save as PDF …" with the shortcut CMD+P. Now, if you print something with CMD+P, a second time pressing CMD+P will open the Save-as-PDF dialog.
* Deactivate TCP to last the Macbook's battery longer: `sudo pmset -b tcpkeepalive 0`

### macOS Tipps

* [Must have macOS Quick Look Plugins](https://sayzlim.net/must-have-macos-quicklook-plugins/)
* [Safari browser with real fullscreen mode](http://www.apfelpage.de/news/mac-tipp-im-safari-browser-mit-echtem-fullscreen-surfen/)
* [Tipps for .bash_profile](https://gist.github.com/stephenll/8762279)
* [Mac Security and Privacy Guide](https://github.com/drduh/macOS-Security-and-Privacy-Guide)
