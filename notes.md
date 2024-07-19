# Lenovo TB-8505FS Hacking

Run the following command to unlock:
```
$ sudo fastboot flashing unlock
```

Run the following command to verify:
```
$ sudo fastboot getvar unlocked
unlocked: yes
```

Rooting guide:
https://www.reddit.com/r/androidroot/comments/l6qasc/how_i_rooted_my_lenovo_tab_m8_research_on_mtk/

Rescue ROMs:
https://drive.google.com/drive/folders/1EzwLL8J6g9ZceZx7_RuFcUwSS9eckk0a

```
fastboot flash vbmeta --disable-verity --disable-verification vbmeta.img
```

GSI roms:
https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list

Working "vanilla" TrebleDroid ROM (system-td-arm64-ab-vanilla.img.xz):
https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20240226

```
sudo ./fastboot erase system
sudo ./fastboot erase userdata
sudo ./fastboot format system
sudo ./fastboot format userdata
sudo ./fastboot flash system system-td-arm64-ab-vanilla.img
sudo ./fastboot reboot
```

