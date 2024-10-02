Metamod plugin to unlock the max player limit on L4D and L4D2.

# Fork
* Form form [accelerator74/l4dtoolz](https://github.com/accelerator74/l4dtoolz)
* Original: https://forums.alliedmods.net/showthread.php?t=93600

# How to install | 如何安裝
* [English](https://github.com/fbef0102/Game-Private_Plugin/tree/main/Tutorial_%E6%95%99%E5%AD%B8%E5%8D%80/English/Server/Install_Other_File#l4dtoolz)
* [中文說明](https://github.com/fbef0102/Game-Private_Plugin/tree/main/Tutorial_%E6%95%99%E5%AD%B8%E5%8D%80/Chinese_%E7%B9%81%E9%AB%94%E4%B8%AD%E6%96%87/Server/%E5%AE%89%E8%A3%9D%E5%85%B6%E4%BB%96%E6%AA%94%E6%A1%88%E6%95%99%E5%AD%B8#%E5%AE%89%E8%A3%9Dl4dtoolz)

# Feature
* LAUNCH OPTIONS
    * Max. clients allowed in your server (Range: 1~31)
    * Max. clients = Human player + AI Bots
        * ```-maxplayers 31```

* CVARS
    * Max human players that can join your server. -1 to disable and use standard check (Range: 1~31)
        ```c
        sv_maxplayers "18"
        ```
    * If set 1, remove lobby reservation, and force to set ```sv_allow_lobby_connect_only 0```
        ```c
        sv_force_unreserved "0"
        ```

# 差別
* 有兩個分支，兩種不同的l4dtoolz檔案
    * master 
        * 最新版本的l4dtoolz，語法翻新重製，使用以下設置時無法從大廳匹配，只能直連
            ```c
            sv_allow_lobby_connect_only 0
            sv_force_unreserved 1
            ```
    * old_l4dtoolz
        * 保留舊版本的l4dtoolz，使用以下設置時依然可以從大廳匹配，也能直連
            ```c
            sv_allow_lobby_connect_only 0
            sv_force_unreserved 1
            ```


