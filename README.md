# Apex Configs
configs optimized for a competitve player and the highest fps posible.

please feel free to contribute in testing, cleaning up or adding posible command tweeks. cvar.txt has many commands to test.

## Start up options
Running on start up using start up options may crash your game. Go by ```profile.cfg``` method if you are having issues. scroll to **Running autoexec on startup**.

You can add these in origin or at the end of your **Target:** path in your desktop shortcut's properties(helps if you have multiple accounts) You can use ```+``` or ```-``` to tag a startup command.

```+fps_max 0 -refresh 240 -forcenovsync -fullscreen -high +exec autoexec.cfg```

```+fps_max``` set fps 1-300.
```-refresh``` add the hz of you monitor's refreshrate.
```-preload``` could cause stutters on some old systems. but will increse preformance on others.
```-high``` is to set the game process in high priority.

#### Running autoexec on startup

If you wish to autoexec on Start up you can add ```exec "autoexec.cfg"``` at the end of ```profile.cfg```. EXAMPLE: [profile.cfg](https://raw.githubusercontent.com/240hz/ApexConfigs/master/profile.cfg) You will need to make ```profile.cfg``` read only or else it will over wright after execution. 


## Locations

```videoconfig.txt``` and ```settings.cfg``` go in 

```C:\Users\ (user) \Saved Games\Respawn\Apex\local```

```videoconfig.txt``` should be set to read only. as making a video change in game will result in the file to reset.

```profile.cfg``` belongs in ```C:\Users\(user)\Saved Games\Respawn\Apex\profile\``` 

```autoexec.cfg```,   ```bind.cfg```, and ```console.cfg```'s belong in the instalations path ```Apex/cfg/```

example ```C:\Program Files (x86)\Origin Games\Apex\cfg\autoexec.cfg```

## Consistant frame caping

Use RTSS for framerate caping as like most other game engines caps nothing beats RTSS in frametime consistancy. I wish there was an equivalent that was open source

https://www.guru3d.com/files-details/rtss-rivatuner-statistics-server-download.html

## Included binds

Included binds in ```binds.cfg``` that is exicuted in ```autoexec.cfg```

 - ```~``` or ``` ` ``` will re-execute ```autoexec.cfg```
 - ```DELETE``` toggles network graph.
 - ```END``` toggles ```cl_showpos 0 1```
 - ```HOME``` toggles ```cl_showfps 0 4```
 - ```=``` toggles master volume 100% 15% ```-``` toggles master volume mute/100%
 - ```MUST ENABLE``` toggles ```cl_fovScale``` (70-120) a fix for bloodhounds ult if you get massive frame drops.

## Other things notable 

- Binding a third key is simple and can be done in ```*.cfg```. for examples reference ```settings.cfg```. Insted of a ```0``` or a ```1``` at the end of the bind command seqence you will need to put a ```2```. For a 4th bind of an action you will need a ```3``` etc. example: ```bind "ALT" "+jump" 2```. This would make the 3rd bind for jump ALT. and this should be put in ```binds.cfg```.

- executing the autoexec.cfg while in a match ```DEL``` key will apply visual diffrences. these visual diffrences are optimized atm for Max Dark Boost options on gaming monitors.

- some command settings only work at startup in ```videoconfig.txt``` like LOD. and others like FOV may work as a ingame bind.

## credits
Multiple reddit post and also githubs. Check out these other configs lots of good examples!

https://github.com/kALLEBALIK/Apex-config

https://github.com/IY/RatzAutoexec

https://github.com/r1ft4469/Apex_Config

https://github.com/NotTsunami/ApexConfig

## to do

- compare against mendo's autoexec when released
- clean up cfgs
