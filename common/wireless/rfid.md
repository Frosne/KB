## RFID
+ "**радиочастотная идентификация** способ автоматической идентификации объектов, в котором посредством радиосигналов считываются или записываются данные, хранящиеся в так называемых транспондерах, или RFID-метках"
<br> &mdash; [Википедия: RFID](https://ru.wikipedia.org/wiki/RFID)

Хотя за rfid как правило считают метки, за rfid можно считать что угодно работающее посредством радиосигналов и позволяющее себя отличить от других, будь то [ble с ibeacon](http://get.openbeacon.org/about.html), [wifi](http://www.huffingtonpost.com/joe-ross/wifi-tracking-when-sniffi_b_5891344.html) или может даже [эллектромагнитное излучение](http://www.rtl-sdr.com/disney-research-em-id-rtl-sdr-based-tag-less-id-of-electrical-devices-via-eletromagnetic-emissions/).

+ ## Железо
Его много, если килогерцовые(LF) метки которые чаще всего используются для пропусков в офисы практически беззащитны и их можно без проблем считывать и записывать подходящим под тип карты ридером, то на HF(13.56МГц) популярностью пользуются ридеры которые хорошо поддерживаются поддерживаются nfc-tools [1](http://nfc-tools.org/index.php?title=Devices_compatibility_matrix)

+ [ChameleonMini](https://github.com/emsec/ChameleonMini/wiki) - Всё в одном, ридер, сниффер, эмулятор.

+ Android устройство с nfc и поддержкой Host-based Card Emulation (HCE).

+ ## Софт
+ [libnfc](https://github.com/nfc-tools/libnfc)
+ [rfidiot](http://rfidiot.org/)

+ ## Дополнительные материалы
+ [2013, Francis Brown, Blackhat RFID-Hacking-Live-Free-or-RFID-Hard](https://media.blackhat.com/us-13/US-13-Brown-RFID-Hacking-Live-Free-or-RFID-Hard-Slides.pdf)
+ [2015, Craig-Young, DEF CON 23, How To Train Your RFID Hacking Tools](https://media.defcon.org/DEF%20CON%2023/DEF%20CON%2023%20presentations/DEFCON-23-Craig-Young-How-To-Train-Your-RFID-Hacking-Tools-WP-UPDATED.pdf)
+ [RFID Zapper](https://ru.wikipedia.org/wiki/RFID_Zapper)
+ [RFID SQL injection](https://ru.wikipedia.org/wiki/RFID-вирус)

