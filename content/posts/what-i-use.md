---
title: Software I Use On Linux 
date: 2025-01-11
tags: ['linux']
---

**[<-- Back]({{< ref "_index.md" >}})**

What I use is pretty standard in the realm of linux. To give some context, I am a novice programmer who enjoys learning about software but whose livelihood does not depend on using development tools. I prefer using terminal-based programs, but I also don't believe that GUI programs are objectively horrible. I mostly need a working operating system where I can do typical computing tasks. If you're reading this, chances are you probably know about all of these programs already and reading on is a waste of time.

## Artix Linux
I've only seriously used three distributions: [Raspbian](https://www.raspberrypi.com/software/), [Linux Mint](https://www.linuxmint.com/), and [Artix Linux](https://artixlinux.org/). I also have a machine that runs Debian, but I almost never use it. Raspbian is understandably slow considering that it must run on a Raspberry Pi. Linux Mint is a really good choice, but I prefer Artix Linux just because of how minimal it is. I definitely couldn't have jumped right into Artix without first using Linux Mint. 

I used have used Artix in the past by installing a [graphical installation image](https://artixlinux.org/download.php), which is such a nice thing. It is essentially Arch Linux with the simple installation of Linux Mint, albeit with unnecessary packages and programs you might not use. I am currently using Artix Linux with the base ISO image, which has its downsides but I have now gotten it up to a point of a graphical installation ISO. Artix doesn't get in your way and is probably what I'll be using for a while.

## dwm
[Dwm (Dynamic Window Manager)](https://dwm.suckless.org/) is a tiling window manager that initially gives you little but can be set up to become an invaluable piece of software. I have used i3 and awesomewm before, but dwm has been my favorite. 

## st
Honestly, being particular about a terminal seems pretty stupid. From my limited point of view as a Linux layman, they all practically do the same thing with some minor strengths and weaknesses. I use [St (Simple Terminal)](https://st.suckless.org/), which is very similar to dwm (another suckless program) in that it also doesn't give much up front. Configuring and rebuilding the program is a cornerstone of suckless software. [Alacritty](https://alacritty.org/) is another terminal emulator that is technically less lightweight than st, but modern computers seem to run them all the same.

Both dwm and st are great pieces of software, but they just need work to set up. I have configured them before from the base-up with patches and such, but I have discovered that using pre-configured versions is a much more efficient use of time. I currently use [chadwm](https://github.com/siduck/chadwm) and Luke Smith's [st](https://github.com/lukesmithxyz/st) build.

## Neovim
Vim is great. It isn't that hard to learn and definitely beats any other GUI text editor for me. [Neovim](https://neovim.io/) seems to be preferred over [vim](https://www.vim.org/) which is preferred over [vi](https://en.wikipedia.org/wiki/Vi_(text_editor)). I've talked about [vim in a previous post]({{< ref "vim.md" >}}), which has more information. 

## Gnome Pomodoro
Using the [pomodoro technique](https://en.wikipedia.org/wiki/Pomodoro_Technique) has proved to be useful in getting stuff done that I'd rather not be doing. [Gnome Pomodoro](https://gnomepomodoro.org/) is probably as straightforward of a timer as you can get. In the future, I want to either find/code a simple pomodoro timer for the terminal or buy a physical timer and track my sessions in a notebook.

## Librewolf
[Librewolf](https://librewolf.net/) and [Ungoogled Chromium](https://github.com/ungoogled-software/ungoogled-chromium) are privacy-centered versions of their respective browsers. I've used both but now use Librewolf.

## Obsidian
[Obsidian](https://obsidian.md/) is closed source, but how it keeps notes in Markdown gives me confidence that I would be able to move away from it if it were to become more intrusive. Before using Obsidian, I never really kept digital notes. Now, I have a scattered collection of notes that makes it useful to refer back to past information.

## Nitrogen
[Nitrogen](https://github.com/l3ib/nitrogen/) is a great wallpaper setter. [Feh](https://feh.finalrewind.org/) can also set the background in a more minimal way, but nitrogen just makes it easier to keep a collection of wallpapers.

## Zathura
[Zathura](https://pwmt.org/projects/zathura/) is a great pdf viewer. I've found that [Atril](https://wiki.mate-desktop.org/mate-desktop/applications/atril/) works better on very large pdf files, but Zathura is more to the point. It uses vim-style keybinds and has little in terms of user interface.

## Calibre
[Calibre](https://calibre-ebook.com/) is pretty bloated, but it performs its purpose well: managing ebooks. It makes organizing ebooks, fetching book covers, and transferring books onto e-readers easier.
