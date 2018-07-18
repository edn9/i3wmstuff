# eyes of hill
My personal and first dotfiles. For this Ricing I used Manjaro with i3 but It can work in whatever distro you want.

------

![Image](https://orig00.deviantart.net/ac43/f/2018/198/8/9/dotfiles_by_necronoise-dchj24w.png)

## Requirements for this desktop

All programs can be found in your distro repository, if not, try searching here in github.

+ WM: i3-gaps ([i3scripts](https://github.com/justbuchanan/i3scripts), i3exit, i3blocks, [betterlockscreen](https://github.com/pavanjadhaw/betterlockscreen))
+ Bar: i3bar (i3status with fontawesome, icomoon, [necrofont](https://github.com/necronoise/necrofont) and autorename_script,this one is with i3scripts)
+ Terminal: urxvt ([urxvt-resize-font](https://github.com/simmel/urxvt-resize-font), `font: TerminessTTF Nerd Font Mono in aur nerd-fonts-terminus`)
+ Colors: [pywal](https://github.com/dylanaraps/pywal)
+ Nitrogen (to make the wallpaper as you desktop wall)
+ [vilfetch](https://github.com/necronoise/vilfetch)
+ ranger
+ mpv
+ compton

## How to

First, the bar: 

+ I use i3bar so... All the colors are in `/home/user/.i3/config`, I did the colors manually.

+ The icons are in the `autorename_workspaces.py`[*](https://github.com/justbuchanan/i3scripts/blob/master/autoname_workspaces.py), `/home/user/.i3scripts/`, I put it manually so to show up in your bar you just need to put the `fonts.ttf` that you downloaded in `.local/share/fonts/` (necrofont ex, the other fonts you can find in your distro repository).

+ The status of the bar are in i3status (you downloaded it with i3-gaps I think) you put in `/etc/i3status.conf` (need sudo), the i3status use fontawesome and icomoon to show up.

Second, the wallpaper. Its pretty simple, just use Nitrogen (or other program) to set up lol. (But remember where is the path of the wallpaper to use in other stages here down below).

The last one, Terminal. 

+ You can use urxvt (or other), all the colors are made with pywal and the wallpaper, its pretty simple, all you need is to open a terminal and write:

> wal -i /home/user/path/to/wallpaper.png

+ Then to make it fix (stay after reboot) you will need to put `wal -r` at the end of the `.xinitrc`. 
+ Also some colors and effects are all in `.Xresources (put it in /home/user/)` and `compton.conf (put it in /home/user/.config/)`.

I also use another script called `resize-font`[*](https://github.com/simmel/urxvt-resize-font) to make the terminal look tiny, it also can serve as zoom in zoom out for the letters, its pretty good! (The font-resize need to be in `/home/user/.urxvt/ext/`.

+ And then, this line in your .Xresources.
> URxvt.perl-ext-common: resize-font

+ Video example of how its gonna look: (soon)

You can alread get all of this config in my files on top of this page. This is just a little tutorial to make it easyer(?) for novice users. Good ricing and good luck!
