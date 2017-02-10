# SDR
> "**Программно-определяемая радиосистема** (англ. Software-defined radio, SDR) — радиопередатчик и/или радиоприемник, использующий технологию, позволяющую с помощью программного обеспечения устанавливать или изменять рабочие радиочастотные параметры, включая, в частности, диапазон частот, тип модуляции или выходную мощность"
<br> &mdash; [Википедия: Программно-определяемая радиосистема](https://ru.wikipedia.org/wiki/Программно-определяемая_радиосистема)

## Железо

Начать можно с тв-тюнера с чипсетом RTL2832U+R820T2 ~7$ на aliexpress в качестве приёмника и raspberry pi c [rpitx](https://github.com/F5OEO/rpitx) в качестве [передатчика](https://www.youtube.com/watch?v=UwgJiUhloho), продолжить на полудуплексном [HackRF](https://greatscottgadgets.com/hackrf/) ~¥1200.00 на taobao или дуплексном [BadeRF](www.nuand.com) ~¥4000.00 либо дождаться [LimeSDR](https://myriadrf.org/projects/limesdr/).

## Софт

- [SDR#](http://airspy.com/download/) -
Хорош за счет большого количества [плагинов](http://www.rtl-sdr.com/sdrsharp-plugins) [[1]](http://rtl-sdr.ru/category/plugin) среди которых удобнейший [timeshift](http://rtl-sdr.ru/uploads/download/timeshift.zip) без которого например услышать разговоры по рации довольно проблематично из-за их зачастую малой продолжительности и невозможности быстро среагировать и подстроить частоту в риалтайме.

- [GQRX](http://gqrx.dk/) -
Значительно меньшее количество плагинов и отсутствие таймшифта делают свое дело, слушать через него сложнее, но производительность значительно лучше чем у SDR#.

- [Fldigi](http://www.w1hkj.com/) -
Комбайн по кодированию\декодированию практически всего что летит до 30МГц. Работает через виртуальный аудиокабель.

- [MultiPSK](http://f6cte.free.fr) -
Аналог Fldigi но поддерживает больше протоколов большую часть которых еще попробуй найди в дикой природе. Поддерживает одновременно до пяти rtl-sdr напрямую. Громоздкий  интерфейс с кучей кнопок на одном экране в комплекте.

- [DSD+](http://wiki.radioreference.com/index.php/Digital_Speech_Decoder_%28software_package%29) -
P25, D-STAR, DMR и прочие радости жизни.

- [GNU Radio](http://gnuradio.org/) - Основное что нужно будет задействовать для полноценного использования SDR.
[Вики](http://gnuradio.org/redmine/projects/gnuradio/wiki)

- [Pothosware](http://www.pothosware.com/) -
Аналог GNU Radio с 3,5 готовыми примерами использования, но несколько удобнее чем GNU 
Radio, стоит попробовать и то и другое.

## Анализ принятого
- [Inspectrum](https://github.com/miek/inspectrum)
- [waveconverter](https://github.com/paulgclark/waveconverter)
- [baudeline](http://www.baudline.com/)
- [audacity](www.audacityteam.org)

## Для android
- [Драйвер](https://f-droid.org/repository/browse/?fdfilter=SDR&fdid=marto.rtl_tcp_andro)
- [SDR Touch](http://sdrtouch.com/)
- [RFAnalyzer](https://github.com/demantz/RFAnalyzer)

## Курсы
- [2014, 2015 by Michael Ossmann. Software Defined Radio with HackRF](http://greatscottgadgets.com/sdr)

## Дополнительные материалы
- [2016, Сергей Полторак, Изучаем GNU Radio при помощи микрофона ](https://geektimes.ru/company/zwave/blog/275174/)
- [2016, Michael Ossmann, Rapid Radio Reversing](https://greatscottgadgets.com/tr/gsg-tr-2016-1.pdf)
- [2014. Balint Seeber, Hacking the wireless world with software defined radio-2.0](https://www.blackhat.com/docs/webcast/07172014-hacking-the-wireless-world-with-software-defined-radio-2.0.pdf)
- [2013, Ilya Samokhin, Простой SDR приёмник на ПЛИС](https://habrahabr.ru/post/204310/)

## Ссылки
- [rtl-sdr.com](http://www.rtl-sdr.com) Большой сайт по SDR. Пожалуй там есть всё что надо если достаточно долго его листать. Особенно не мешает посетить вкладку Software=>Experimental Drivers которая добавит новые плюшки вроде расширения диапазона принимаемых частот в RTL2832U+R820T2.
- [Signal Identification Guide](www.sigidwiki.com/wiki/Signal_Identification_Guide)  Образцы сигналов.  Поможет опознать пойманное и понять что и на каких частотах искать.
- [GNU Radio module and Wireshark dissector for the Nordic Semiconductor nRF24L Enhanced Shockburst protocol](https://github.com/BastilleResearch/gr-nordic)

