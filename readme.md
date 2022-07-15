## csgo-cfg
### 游戏启动使用的 cfg  
`csgo.cfg`  
用法:  
在启动项添加
```cfg
+exec csgo.cfg
```  
具体内容
```cfg
//飞行
bind "\" "noclip"
//跳投
bind "n""+jump;-attack;-attack2;-jump"
//大跳
alias +cjump "+jump; +duck"
alias -cjump "-jump; -duck"
bind "space" "+cjump"
//重复投掷物
bind "/" "sv_rethrow_last_grenade"
//清除血迹
bind "shift" "+speed;r_cleardecals"
//移动原有bot，必须场内存在bot
bind "]" "bot_place"
//投掷物绑定
bind "4" "use weapon_hegrenade"
bind "5" "use weapon_flashbang"
bind "c" "use weapon_smokegrenade"
bind "x" "use weapon_molotov;use weapon_incgrenade"
bind "z" "use weapon_decoy"
//一键丢包
bind "t" "use weapon_c4;dorp weapon_c4"

```
------
### 跑图训练使用的 cfg  
`throw.cfg`  
用法:
游戏内进入地图后打开控制台
```cfg
exec throw
```
```cfg
sv_cheats 1
mp_startmoney 16000;
mp_buy_anywhere 1;
mp_buytime 999999;
mp_freezetime 0;
mp_restartgame 1;
sv_infinite_ammo 1;
mp_roundtime_defuse 60;
sv_grenade_trajectory 1;
sv_grenade_trajectory_time "5";
mp_humanteam any
mp_autoteambalance 0;mp_limitteams 0
bot_stop 1
```