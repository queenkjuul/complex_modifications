# complex_modifications (Karabiner-Elements)

Because macOS kinda sucks, and I needed to be able to bring over some of my Windows and Linux workflow

I never figured out how Karabiner decides to read these files--I tried putting in my own random numbers, but they didn't work if I recall correctly, so in the end I just ended up using one imported from the official repo and then modifying them. Not sure what julie.json used to be, scroll.json is a modified version of ["Change Mouse Motion to Scroll (Rev 2)](https://ke-complex-modifications.pqrs.org/#mouse_motion_to_scroll)

## julie.json

all of my custom modifications for Karabiner-Elements that I mostly wrote myself, but borrowed some of the code from existing sets in the Karabiner repo. 

### Shift+Delete

One of the things I hate about Macs is the trash can, and the fact that I cannot quickly delete files permanently like I can in Windows and Linux (using shift+delete). I go through tons and tons of temporary files for work on my Mac, like screenshots and log files, that should not be kept for privacy reasons. 

This remaps `shift+delete` to `control+command+shift+option+K`. The latter combo is then set up to run an Automator workflow that `rm -rf`'s whatever files are selected in Finder. Workflows on Mac are slow, but it works well. 

### Paste and Match

On Windows, `control+shift+V` would paste without formatting. Mac can do this, but it is the cumbersome `command+shift+option+V` combo, which I could not find a way to change. This remaps the former to the latter. 

### Control-W

In Chrome (and I assume any other Mac browser) you use `control+tab` to switch tabs, but you have to use `command+W` to close the tab. Moving my thumb from control to command annoyed me, so I remapped this so that I can navigate and close tabs all on the control key. 

This caused a problem, though, because I had only remapped `control+W` to `command+W`. In `nano`, I would hit control+W to search, then accidentally close my terminal. So this also remaps `option+W` to `control+W` so that I can still use those combos. 

### Control+A/D  -  Desktop Switching

I also hated that the default combo to swap virtual desktops in macOS required me to take my hand off the mouse (the default is `control+left_arrow/right_arrow`). So I remapped `control+A` and `control+D` to the defaults so that I could use either one. This is kind of useless now that I use a non-Apple mouse, but it's good to have. 

### Control+Space [NONFUNCTIONAL]

I really like on Windows 10 how easy it is to pull up the emoji/special characters window with `control+space`. On Mac, it's `control+command+space` which is much harder to hit with your hands in typing position. However, this modifier never worked. 

### Home and End keys

Took this from a set on the main repo. I merged it into this file because it just seems much easier to manage all my customizations from one single file, especially with how often I need to modify the "stock" ones from the main repo. Makes Home and End function like Windows. That's it. 

## scroll.json

This is modified from the ["Change Mouse Motion to Scroll (Rev 2)](https://ke-complex-modifications.pqrs.org/#mouse_motion_to_scroll) modification. I was ECSTATIC to learn that this was a usable option, it was one of the things I missed the most from Windows. However, once I did use it, it broke my ability to use `Mouse3` as a middle-click to open links in new tabs. This fixes that. 