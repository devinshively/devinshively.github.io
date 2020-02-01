---
layout: post
title:  "MacBook Pro Setup"
description: "A guide to setting up my macbook pro
date:   2015-02-28 01:11:36 -0800
categories: "Development" "Setup" "IntelliJ IDEA" "Sublime Text 3" "iTerm"
---

Whether it is a new rig at work or if I messed up my hackintosh install, it is always a pain to remember everything that I have installed. So I thought it would be a good idea to publish my setup for future reference. Most of my setup is pulled and modified from others so credit goes to those before me. I will try to keep this page updated with any changes.

[Alt font](http://www.marksimonson.com/fonts/view/anonymous-pro)

## Sublime Text 3
 - Package Manager:

    ctrl + ` and enter

    ```
    import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
    ```

 - Subl Command line:

    ```
    sudo ln -s "/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl" /usr/bin/subl
    ```

 - Alignment
 - ApplySyntax
 - BracketHighlighter
 - Color Highlighter
 - Colorpicker
 - DocBlockr
 - [Dock Icons](https://github.com/jamiewilson/predawn/tree/master/dock-icons)
 - Emmet
 - GitGutter
 - GoSublime
 - Keybinding:

    ```
    [
        {
            "keys": ["ctrl+shift+r"],
            "command": "reindent",
            "args": { "single_line": false }
        }
    ]
    ```

 - Levels:

   - `ctrl + shift + l` to show colors
   - `ctrl + shift + 0` to normal view

 - MarkdownEditing
 - Sass
 - SCSS
 - SidebarEnhancements
 - SublimeLinter
 - Tag
 - Themes:

    Solarized Dark (my current), Soda, Flatland, Predawn, Spacegray

 - TrailingSpaces


## IntelliJ Idea

I backup my settings to Cloud Station as settings.jar

Go to File > Import Settings... and select settings.jar

<br />
To install Solarized Dark Theme first download the [settings.jar](https://github.com/jkaving/intellij-colors-solarized)

Go to File > Import Settings... and select settings.jar

Restart IntelliJ IDEA

Go to Appearance > Theme and select Darcula

Go to Preferences > Editor > Colors & Fonts and select Solarized Dark (Darcula)

## Homebrew
 - Install homebrew

    ```ruby
    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    ```

 - Install packages

    ```
     brew doctor
     brew install go
     brew install node
     brew install vim --override-system-git
     brew install git --override-system-git
     brew install gradle
     brew install python3; pip3 install --upgrade pip
     ```

## npm
 - Update npm and install global packages

    ```
     npm install -g npm@latest
     npm install -g bower
     npm install -g nodemon
     npm install -g sails
     ```

## sql developer
 - Import connections xml

## iterm2
 - [Font 15pt Source Code Pro Light for Powerline](https://github.com/Lokaltog/powerline-fonts/tree/master/SourceCodePro):

    iTerm > Preferences > Profiles > Text and select Change Font

    Select Source Code Pro Light 15pt

 - [Solarized Dark Theme](http://ethanschoonover.com/solarized/files/solarized.zip):

    iTerm > Preferences > Profiles > Colors and Load Presets...

    Select solarized/iterm2-colors-solarized/Solarized Dark

    Select Load Presets... and select Solarized Dark
 - Cursor:

    #d13a82

## p4v
 - Setup workspace

## hipchat

## sourcetree

## Xcode
 - Alcatraz:

    ```
    curl -fsSL https://raw.github.com/supermarin/Alcatraz/master/Scripts/install.sh | sh
    ```

 - Solarized Dark Theme:

    Installed through Alcatraz Window -> Package Manager

 - CocoaPods:

    Insatlled through Alcatraz Window -> Package Manager

## mongodb
 - Install mongodb:

    ```
    brew install mongodb
    ```

 - Make data directory:

    ```
    sudo mkdir -p /data/db
    sudo chown dshively /data/db
    ```

## Google Chrome
I use Google Chrome main build with the following extensions:

- Web Server Notifier
- Web Technology Notifier
- Chrome Sniffer
- Ultimate User Agent
- What Font?
- Clear Cache
- REST Client
- Rails Panel
- Edit Cookie
- jQuery debugger
- XV XML
- JSON formatter
- PrettyPrint
- CSSViewer
- Chroma
- Live Reload
- Pages Speed

## tomcat 7.0.57

## servicemix 5.1.4

## ant 1.9.4

## maven 3.2.3
 - Copy maven settings.xml file from repo to ~/.m2

## spectacle

## alfred

## f.lux

## ~~dropbox~~ CloudStation
Since purchasing a Synology DiskStation I now use CloudStation
