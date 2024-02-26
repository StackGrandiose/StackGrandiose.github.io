---
title: Using Vim
date: 2023-07-28
tags: ['vim', 'linux']
---

**[<-- Back]({{< ref "_index.md" >}})**

## My Experience Using Vim

Around the start of June, I went through the trouble of installing Artix Linux on a laptop. With this, I had the choice of what text editor I could install onto my system. In the past, I have never really done any true programming work or config editing on my previous desktop Linux Mint machine. In the occasion that I did, however, I must have used a default text editor like xed. This style of usage really discouraged any sort of terminal work, which would be suited to using vim. I must have heard about vim in the past, and heard about its efficiency when working and its keyboard centric control. So, I installed vim and began my learning process.

_At the time of writing, I am not someone that programs regularly and cannot speak well for its functionality as a IDE. This is just my experience using vim casually for various tasks._

Vim is operated through different "modes" which allow you to do different actions. "Normal" mode is usually where you enter in commands to do various actions. "Insert" mode is exactly what it sounds like and doesn't allow you to do much else except hit the keyboard and type text. "Visual" mode works similarly to GUI text editors and allows you to select text. Vim's effeciency comes through using this modal system and allows you to execute specific key combinations to do exactly what you intend to do. Many actions that a mouse would normally do is replaced with keys. Instead of scrolling, you can use `hjkl` for going line-by-line, `ctrl + u` and `ctrl + d` for going up and down half a page, go to the top with `gg`. go to the bottom with `G`, move the screen so the cursor is in the middle with `zz`, and more. This fine control over what you can do allows you to forego the aiming of a mouse. Everything you want to can be performed by muscle memory keypresses. 

The need to learn this system is probably a reason for people being hesitant to starting to use vim. However, I think the time used to learn vim is at least more productive than participating in any other of the common time-waster activities. It was pretty easy to learn and did not require difficult memorizing. I started operating vim with a very limited number of actions I knew and gradually learned more to the point where now I can say that I can do a decent amount of stuff I want. I certainly have not learned everything that vim can do, but through using it, you learn more and more. 

I eventually switched to using neovim for its additional features. I followed the ThePrimeagen's configuration guide to add various plugins and themes. It has worked out pretty well and has added some features that make using vim more comfortable. The differences between vim and neovim are not huge but research online will provide you with differences that make neovim the better choice over the two. 

I have been using vim at the moment for editing configuration files, system files, learning c and writing this web page you have been reading this on. Using neovim's telescope, syntax highlighting, and LSP has made all of these tasks pleasent. I tried using vim whilst using Debian in a graphical desktop environment and it just wasn't worth the hassle of switching back and forth from using the keyboard in vim to doing stuff in a file manager. There are graphical vim forks, but I have not tried them and cannot vouch for their usability. Using a tiling WM with vim seems natural while using vim whilst also using a mouse is uncomfortable. You can avoid this possible usage conflict by using vim-like keybindings for your existing text editor.

Using vim has been pretty enjoyable to use for casual text editing. Everyone should at least try out vim-style keybindings or test out vim to see if it is perferable to any existing system they have in place. 

