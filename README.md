# Gargoyle-Luci
    Supported Luci Web Interface in Gargoyle
    Origin source:(https://github.com/ericpaulbishop/gargoyle.git)
## Part ⅰ:
### add luci package from Luci source:
    ./scripts/feeds update luci && ./scripts/feeds install luci
## Part ⅱ:
### custom enter for Gargoyle Web to enter luci Interface:
  package/gargoyle/files/www/overview.sh
##translate for custom laguages:
### For Englist
    package/plugin-gargoyle-i18n-English-EN/files/www/i18n/English-EN/overview.js
    inser "ovwS.Enter="Openwrt Web Interface";" 
### For ZH-CN:
    package/plugin-gargoyle-i18n-SimplifiedChinese-ZH-CN/files/www/i18n/SimplifiedChinese-ZH-CN/overview.js
    inser "ovwS.Enter="Openwrt界面入口";" 
