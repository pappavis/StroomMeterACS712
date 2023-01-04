Zet de voeding aan met Octoprint vlak voor starten met printen.

# Intro
De bedoeling is om een 230V AC middels software te kunnen aan/uitzetten.  In principe kunt je dit gebruiken waar je AC stroom willen aan/uitzetten en meten. Het functioneert in principe dezelfde als een Sonoff POW switch.

# Benodigheden
De volgende heb je nodig;

|Aantal|Item|Kosten|Optioneel|
|------|----|------|---------|
|1x|<a href="https://nl.aliexpress.com/item/1005004344359250.html?spm=a2g0o.cart.0.0.6ca561d7aq0PVO&mp=1&gatewayAdapt=glo2nld">ESP32 S2 Mini</a>|€2,28|N|
|1x|<a href="https://nl.aliexpress.com/item/32949264545.html?spm=a2g0o.productlist.main.1.1964577aTEmXD6&algo_pvid=6153c03f-b4b4-4653-a854-14e6c40e5aa0&aem_p4p_detail=202301040356468264624950022100000543353&algo_exp_id=6153c03f-b4b4-4653-a854-14e6c40e5aa0-0&pdp_ext_f=%7B%22sku_id%22%3A%2266268030503%22%7D&pdp_npi=2%40dis%21EUR%211.11%211.11%21%21%21%21%21%402145288516728334064801617d0767%2166268030503%21sea&curPageLogUid=MFJIrYuofizE&ad_pvid=202301040356468264624950022100000543353_1&ad_pvid=202301040356468264624950022100000543353_1">ACS712-05</a> breakout board|€1,11|N|
|1x|<a href="https://nl.aliexpress.com/item/32808620818.html?spm=a2g0o.order_list.order_list_main.5.2b0a79d2QUDt5m&gatewayAdapt=glo2nld">SRD-03VDC-SL-C 10A 250V</a> relay|€2,44|N|
|1x|<a href="https://nl.aliexpress.com/item/32672327708.html?spm=a2g0o.cart.0.0.5e6f61d7sThdsn&mp=1&gatewayAdapt=glo2nld" target="_blank">Oled 128X32</a>|€1,38|J|

Je kunt van Aliexpress bestellen die in één pakketje worden opgestuurd.

#Hoe werkt het
TODO: onderstaand schema uitleggen.

<img src="https://github.com/pappavis/StroomMeterACS712/blob/main/img/Aan-uit_relay_schakeling_20211006_Max50.jpg?raw=true" width="30%" height="30%">


Geïnspireerd door
 * <a href="https://www.youtube.com/watch?v=dQNBeAZpRmk" target="_blank">Deze</a> videoclip.
 * OctoPrint <a href="https://plugins.octoprint.org/plugins/psucontrol/" target="_blank">psucontrol</a> uitbreiding.

door: 2023 #easylab4kids
