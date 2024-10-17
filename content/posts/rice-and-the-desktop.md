+++
date = '2024-10-16T21:13:28-06:00'
draft = false
title = 'Rice and the Desktop'
tags = ["ricing"]
+++

I'm currently in the process of customizing my linux desktop, what the cool kids call "ricing."
It's fun but I feel I need to lay out the whole process, and what I want to do somewhere, so like a sane person I spun up a blog to write it out on.
Honestly this post is mostly for me, but if you want to learn about ricing, look at this [other person's post](https://namishh.me/blog/ricing/).
So anyway, let's get on with it!

## Overall Goals and Philosophy

Overall I want to make a desktop where I'm comfortable and common tasks are a couple keybinds away.
So here are my main goals:

- Intuitive (to me) system of key binds
- Can be easily copied to another computer
- aesthetic 

I also have a bit of a minimalist philosophy when it comes to designing this.
Not to say I won't have lots of features, but I'll consider if I really need them.
If I'm not going to use it, I don't really want it on my screen or taking up key binds.

In addition I love NeoVim and will use it every chance I get; It's what I'm writing this post in now!

## What I have so far

![desktop_sample](../images/rice-and-the-desktop/desktop_sample.png#center)
![desktop_sample2](../images/rice-and-the-desktop/desktop_sample2.png#center)

It looks alright, still have some theming work to do on some applications though.
I love the partially transparent terminal though, my absolute favorite.

Listing what I'm using for all the components, I've got:
- hyprland (tiling window manager)
- alacritty (terminal)
- tmux (terminal multiplexer)
- ags (desktop widgets i.e. the clock and the workspace display at the bottom center of screen, also does notifications)
- neovim (text editor)
- rofi (application picker)
- nwg-hello (greeter)

I like to have workspaces 1,2,3,4, and 5 on my left monitor and 6,7,8,9, and 0 on my right.
As such I have it automatically set up to only place them on those monitors, and move me to the appropriate monitor when I change workspace.

Now I'm going to list some flaws in my current setup
- Notifications often get stuck on screen
- I haven't setup the media buttons on my keyboard to work
- I don't like how nwg-hello looks
- I'm not sure how I want my lock screen to look
- My key binds are random and suck (why is open terminal ctrl-z?)
- I really want meta-j and meta-k to move workspaces if I'm at the bottom or top window.

These will motivate the next sections.

## To AGS or not to AGS

So AGS is a framework for writing your own desktop widgets.
I spent a little too much time customizing it for mine, so I don't really want to just give it up.
But at the same time something like waybar may be the best option.
I need to look into it more, but AGS should probably be avoided unless I want to do something waybar can't do.
If I leave AGS I'll need a new notification daemon, but that shouldn't be that hard to get.

## Key Binds

I use several programs with their own particular approaches keybind : NeoVim, Tmux, probably something else I'm not thinking of.
As such I want to match my approach to keybinds with theirs.
Specifically in Tmux you press a prefix key and then your next input is a tmux command.
I think I can emulate this in hyprland, by doing modes.
So pressing meta-space will bring me into a command mode, then I can press another button to execute that command.
I'll list my current thoughts on keybinds in the command mode below.
- meta-space again brings up my application picker, as it's the default option I want
- 1234... changes to the specific 
- d closes the window (to match with ctrl-d closing terminals)
- meta-hjkl moves left down up or right depending on which key (like in NeoVim)
- meta-j and meta-k get really special functionality allowing them to move up and down windows, but also up and down workspaces when I reach the top or bottom of screen.
- probably a keybind to go to my dnd notes, or make a new note (I'm always so slow about opening them when we start playing)

I also want keybinds along the lines of what [Gilles Castel](https://castel.dev/), may he rest in peace, had for his setup.
That is keybinds with calendar integration to check what class I'm currently in and open my latex notes for that class.

## Aesthetics (totally can spell that without googling it)

I should talk to some other people and get their thoughts on how to do my lock screen and status bar and stuff.
Cause IDK.

## Conclusion

This was very helpful for me, and that's all that matters.
F*** you.
