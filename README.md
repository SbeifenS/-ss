# Gargoyle-Luci
    Supported Luci Web Interface in Gargoyle
    Origin source:https://github.com/ericpaulbishop/gargoyle.git
## Part ⅰ:
### add luci package from Luci source:
    ./scripts/feeds update luci && ./scripts/feeds install luci
## Part ⅱ:
### custom enter for Gargoyle Web to enter luci Interface:
  replace package/gargoyle/files/www/overview.sh
### link Gargoyle Web from luci Interface: 
    feeds/luci/themes/luci-theme-bootstrap/luasrc/view/themes/bootstrap/header.htm
    change line 117 as: <a class="brand" href="/login.sh"><%=boardinfo.hostname or "?"%></a>
##translate for custom laguages:
### For Englist
    package/plugin-gargoyle-i18n-English-EN/files/www/i18n/English-EN/overview.js
    inset "ovwS.Enter="Openwrt Web Interface";" 
### For ZH-CN:
    package/plugin-gargoyle-i18n-SimplifiedChinese-ZH-CN/files/www/i18n/SimplifiedChinese-ZH-CN/overview.js
    inser "ovwS.Enter="Openwrt界面";" 
## Part ⅳ：
    ###change default target config files(gargoyle/taget/ar71xx/profile/usb_large_nand)
        set gargoyle-plugin-SimplifiedChinese-ZH-CN as build-in plugin by modify "m" to "y"
