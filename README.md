# StroomMeterACS712
Measure AC power usage using ESP8266 and ACS712

Work in progress!!  Nothing to see here, not yet.

<img src="https://github.com/pappavis/StroomMeterACS712/blob/main/img/ACStroommeter_schema.jpg?raw=true" width="60%" height="60%" title="schema">

# Benodigheden
De volgende heb je nodig;

|Aantal|Item|Kosten|Optioneel|Data / info|
|------|----|------|---------|--|
|1x|<a href="https://nl.aliexpress.com/item/1005004344359250.html?spm=a2g0o.cart.0.0.6ca561d7aq0PVO&mp=1&gatewayAdapt=glo2nld" alt="MCU verplicht">ESP32 S2 Mini</a> met Bluetooth &amp; WiFi|€2,28|N|<a href="https://www.wemos.cc/en/latest/s2/s2_mini.html">datasheet</a>|
|1x|<a href="https://nl.aliexpress.com/item/32949264545.html?spm=a2g0o.productlist.main.1.1964577aTEmXD6&algo_pvid=6153c03f-b4b4-4653-a854-14e6c40e5aa0&aem_p4p_detail=202301040356468264624950022100000543353&algo_exp_id=6153c03f-b4b4-4653-a854-14e6c40e5aa0-0&pdp_ext_f=%7B%22sku_id%22%3A%2266268030503%22%7D&pdp_npi=2%40dis%21EUR%211.11%211.11%21%21%21%21%21%402145288516728334064801617d0767%2166268030503%21sea&curPageLogUid=MFJIrYuofizE&ad_pvid=202301040356468264624950022100000543353_1&ad_pvid=202301040356468264624950022100000543353_1" alt="AC stroom meten tot 20A">ACS712-05</a> breakout board|€1,11|N|<a href="https://octopart.com/datasheet/acs712elctr-05b-t-allegro+microsystems-38944601">datasheet</a>|J|
|1x|<a href="https://nl.aliexpress.com/item/32808620818.html?spm=a2g0o.order_list.order_list_main.5.2b0a79d2QUDt5m&gatewayAdapt=glo2nld">SRD-03VDC-SL-C 10A 250V</a> relay|€2,44|N|<a href="http://www.datasheetcafe.com/srd-05vdc-sl-c-datasheet-pdf/" alt="verplicht. aan uit schakelaar">datasheet</a>|
|1x|I2C <a href="https://nl.aliexpress.com/item/32672327708.html?spm=a2g0o.cart.0.0.5e6f61d7sThdsn&mp=1&gatewayAdapt=glo2nld" target="_blank">Oled 128X32 scherm</a>|€1,38|J|datasheet|
|1x|<a href="https://nl.aliexpress.com/item/1005003568092031.html?spm=a2g0o.productlist.main.7.30e378e19RwleU&algo_pvid=45aa2b55-53f0-4cf6-be4c-6e9c11d61f6f&aem_p4p_detail=202301040503385945494397516960000675494&algo_exp_id=45aa2b55-53f0-4cf6-be4c-6e9c11d61f6f-3&pdp_ext_f=%7B%22sku_id%22%3A%2212000030654022470%22%7D&pdp_npi=2%40dis%21EUR%215.04%213.93%21%21%21%21%21%402145265416728374183238677d0782%2112000030654022470%21sea&curPageLogUid=Hf4C5MspqKPZ&ad_pvid=202301040503385945494397516960000675494_4&ad_pvid=202301040503385945494397516960000675494_4">SPDT</a> tuimelschakelaar|€0,10|N|<a href="https://www.electronicshub.org/switches/" alt="hulp artikel">info</a>|
|1x|I2C <a href="https://nl.aliexpress.com/item/1005001682363363.html?spm=a2g0o.productlist.main.1.59bf3ddaYob59r&algo_pvid=b5a2e4fa-2b1d-4794-aa8b-f1d2eecffdef&aem_p4p_detail=202301040508292990992845371040000686338&algo_exp_id=b5a2e4fa-2b1d-4794-aa8b-f1d2eecffdef-0&pdp_ext_f=%7B%22sku_id%22%3A%2212000017115738926%22%7D&pdp_npi=2%40dis%21EUR%211.97%211.97%21%21%21%21%21%402145265416728377092613039d0782%2112000017115738926%21sea&curPageLogUid=OZkt1SVUV4Va&ad_pvid=202301040508292990992845371040000686338_1&ad_pvid=202301040508292990992845371040000686338_1">PCF8574P</a> 8-bit expander|€0,20|N|<a href="https://github.com/mcauser/micropython-pcf8574">info</a>|

Je kunt van Aliexpress bestellen die in één pakketje worden opgestuurd.

# Waarom?
De bedoeling is om een 230V AC middels software te kunnen aan/uitzetten.  In principe kunt je dit gebruiken waar je AC stroom willen aan/uitzetten en meten. Het functioneert in principe dezelfde als een Sonoff POW switch.

# Hoe werkt het
Wanneer IO-pin HIGH op de ESP32 gaat de voeding aan, aangestuurd door Octoprint, vlak voor starten met printen.

TODO: onderstaand schema uitleggen.<br>
<img src="https://github.com/pappavis/StroomMeterACS712/blob/main/img/Aan-uit_relay_schakeling_20211006_Max50.jpg?raw=true" width="30%" height="30%"><br>
Credits: Max50

# Geïnspireerd door
heb de kunstje beetje afgekeken van;
 * <a href="https://www.youtube.com/watch?v=dQNBeAZpRmk" target="_blank">Deze</a> videoclip.
 * OctoPrint <a href="https://plugins.octoprint.org/plugins/psucontrol/" target="_blank">psucontrol</a> uitbreiding.

# Algemeen foto's
ACS712 breakout board &amp; <a href="https://octopart.com/datasheet/acs712elctr-05b-t-allegro+microsystems-38944601" target="_blank">datasheet</a>:<br>
<img src="https://github.com/pappavis/StroomMeterACS712/blob/main/img/acs712_breakout.jpg?raw=true" title="acs712_breakout"/></img>
<br>

Tip: PCB gcode voor jouw CNC machine kunt je genereren voor met <a href="http://flatcam.org" target="_blank">Flatcam.org</a>

Credit: <a href="https://www.youtube.com/@easylab4kids246" target="_blank">#easylab4kids</a>

