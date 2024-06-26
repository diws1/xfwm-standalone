# xfwm-standalone

## Why xfwm ?
xfwm has the all window manager features i need. Like most window managers, I just had to add a few things to make it ready to use, and it was even easier in my opinion.

## How to install xfwm ? 
xfwm is generally provided by the package <b>xfwm4</b>.
```
sudo apt install xfwm4
```

to get started, you can start xfwm with a display manager. in this case i use <b>lightdm</b>, so i need to create [<b>xfwm4.desktop</b>](https://github.com/diws1/xfwm-standalone/blob/main/usr/share/xsessions/xfwm4.desktop) file on my <b><i>/usr/share/xsessions/</i></b> directory.
```
sudo nano /usr/share/xsessions/xfwm4.desktop
```

<b>xfwm has three setting options by default :</b>
- <b>xfwm4-settings</b> for theme and shortcuts
- <b>xfwm4-tweaks-settings</b> for compositor
- <b>xfwm4-workspace-settings</b> for workspace and gaps

> [!NOTE]
> <b>xfwm4-settings</b> can't be used as an apps launcher, so i need to install <b>sxhkd</b> for that.
```
sudo apt install sxhkd
```

The last step is to create the autostart file. I use <b>Debian</b> and <b>lightdm</b> as display manager, so I need to create the [<b>.xsessionrc</b>](https://github.com/diws1/xfwm-standalone/blob/main/.xsessionrc) file, and enter <b>sxhkd</b> into it. 
```
sudo nano ~/.xsessionrc
```

##

### preview
![My Image](https://github.com/diws1/xfwm-standalone/blob/main/screenshots/xfwm_idle.png)
my xfwm when idle\
\
\
![My Image](https://github.com/diws1/xfwm-standalone/blob/main/screenshots/xfwm_menu.png)
besides using sxhkd as an launcher, i also use rofi\
\
\
![My Image](https://github.com/diws1/xfwm-standalone/blob/main/screenshots/xfwm_termdir.png)
only shows you when some apps are opened\
\
\
![My Image](https://github.com/diws1/xfwm-standalone/blob/main/screenshots/xfwm_tilling.png)
xfwm tilling, yups you can make xfwm like tilling window manager just using the <i><b>xfwm4-workspace-settings</b><i/>\
\
\
![My Image](https://github.com/diws1/xfwm-standalone/blob/main/screenshots/xfwm_themes.png)
all the theme that i use on this config, thanks for all creators !!!


### another polybar theme
![My Image](https://github.com/diws1/xfwm-standalone/blob/main/screenshots/xfwm_idle2.png)
you can choose polybar themes in my other [repos](https://github.com/diws1/polybar-theme) :)
