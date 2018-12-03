# Gacha
[![Spigot 1.13.2](https://img.shields.io/badge/Spigot-1.13.2-brightgreen.svg)](https://www.spigotmc.org/wiki/spigot/)
[![GitHub release](https://img.shields.io/github/release/kubotan/Gacha.svg)](https://github.com/kubotan/Gacha/releases)
[![Build Status]( https://travis-ci.org/kubotan/Gacha.svg?branch=master)](https://travis-ci.org/kubotan/Gacha)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/kubotan/Gacha/issues)
[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://github.com/kubotan/Gacha/blob/master/LICENSE)

This is a plugin for Minecraft.

# Installation method
Please put jar in the plugins folder of spigot or bukkit.   

Note: It is recommended that you use a protection plug-in such as LWC or WorldGuard.  

# Useage
1. Create signbord.  
line1 `[gacha]` Fixed character string  
line2 `gacha1` Specify gacha name.(Please enter the this line with one-byte alphanumeric underscore.)
line3 `***gacha1***` Title for sign.  
line4 `test gacha` Comment for sign.  

2. Set Chest.
/gacha modify gacha1

Please right click and punch the chest.
After setting the chest, it is completed.
Hold the ticket on your right hand and right click on the signbord to receive the prize.

3. Command.
```
/gacha list - List all gacha
/gacha modify <gacha_name> - Modify a gacha
/gacha delete <gacha_name> - Delete a gacha
/gacha ticket <player_name> - Issue a ticket
```

# Permission
```
gacha.list - /gacha list
gacha.modify - /gacha modify
gacha.delete - /gacha delete
gacha.create - create gacha by signbord
```
Other operation is op.
Issue ticket is console or op.

# Disclaimer
Do not assume any responsibility by use. Please use it at your own risk.

# Build command(Linux)
```
mvn package
```

# Japanese　日本語φ(｀д´)ﾒﾓﾒﾓ...
→看板を貼り付ける
　1行目「[gacha]」
　2行目「gacha1」       ガチャガチャ設定名（削除や変更で指定する為の名称です。名称には半角英数字とアンダーバーが使えます。）　
　3行目「新規ガチャ」   　ガチャガチャ表示名（看板を貼り付け終わると看板の１行目に表示されます。）
　4行目「初心者装備GET!」 ガチャガチャ説明（看板を貼り付け終わると看板の２行目に表示されます。）
→ガチャ用チェストを設定する
　/gacha modify gacha1
→ガチャガチャ券を発行する
　/gacha ticket kubotan
→右手にガチャガチャ券を持って、先ほど貼り付けた看板を右クリックすると、
　ガチャガチャ券と引き換えに、ガチャ用チェストのどれかアイテム１つがランダムでゲットできます。