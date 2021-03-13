# Начальная настройка цифровой системы DJI FPV System

**Оригинал:** [How Setup DJI FPV System for the First Time](https://oscarliang.com/dji-fpv-system-setup/)

## Включаем FPV очки

- Устанавливаем антенны; убедитесь, что они хорошо закручены

- Подключаем к комплектному кабелю LiPo аккумулятор 3 или 4S

- Одеваем очки, подстраиваем межзрачковое расстояние (слайдеры снизу) проверяем изображение, оно должно быть четким

- Если хотите записывать видео на земле (в очках), тогда вставляем MicroSD карточку в соответствующий слот

![power](/first-steps/pics/dji-fpv-system-power-fpv-goggles-battery.jpg?raw=true)

## Активируем

Открываем https://www.dji.com/ru/fpv выбираем **Скачать**, скачиваем последнюю версию **DJI Assistant 2**. Устанавливаем скачанную программу.

Включаем очки, затем подключаем их к компьютеру комплектным кабелем USB-C.

![cable](/first-steps/pics/dji-fpv-system-fpv-goggles-usb-c-cable-connect-computer.jpg?raw=true)

Запускаем **DJI Assistant 2** и входим в свой аккаунт DJI. Или создаем новый (sign up), если у вас его нет.

![login](/first-steps/pics/dji-fpv-system-dji-assistant-login.jpg?raw=true)

Находим иконку с надписью «DJI FPV goggles» (Очки DJI). Если она не появилась, тогда переподключаем USB кабель. Учтите, что при первом подключении очков компьютеру может потребоваться пара минут для установки драйверов.

Нажимаем на иконку, вас попросят активировать устройство. **Убедитесь, что компьютер подключен к интернету!**

![assistant](/first-steps/pics/dji-fpv-system-dji-assistant.jpg?raw=true)

Каждое устройство активируется отдельно, но шаги те же самые. Так что повторяем активацию для воздушного модуля и для пульта управления.

## Устанавливаем воздушный модуль (air unit)

Если вы собираете дрон с нуля и используете DJI FPV, то лучше всего использовать раму, специально предназначенную для этой системы. Обычно она идет с напечатанными деталями для упрощения крепления воздушного модуля и антенн.

![frame](/first-steps/pics/dji-fpv-system-martian-install-air-unit.jpg?raw=true)

## Подключаем воздушный модуль к полетному контроллеру

Если у вас полетный контроллер специально предназначенный для работы с DJI Air Unit, то просто соединяем их шлейфом и не заморачиваемся разными схемами подключения 🙂 Но если же вы не хотите тратить деньги на новый ПК, то ниже я покажу как соединить воздушный модуль и имеющийся полетник.

![frame](/first-steps/pics/newbeedrone-f4-fc-30a-esc-stack-DJI-Air-Unit-Digital-FPV-System-connected.jpg?raw=true)

Воздушный модуль можно питать напряжением 7,4 — 17,6 вольт, т.е. напрямую от [трех или четырех баночного аккумулятора](https://blog.rcdetails.info/kakie-byvayut-lipo-akkumulyatory-rukovodstvo-dlya-nachinayushhih-pilotov-dronov-i-kopterov/).

Однако, я советую использовать внешний преобразователь напряжения или BEC в полетном контроллере, т.к. скачки напряжения от моторов и регуляторов могут повредить воздушный модуль (так же, как и аналоговый видеопередатчик). [Установка конденсатора достаточной емкости тоже может помочь](https://blog.rcdetails.info/kondensatory-dlya-filtratsii-shumov-v-mini-kopterah/).

![unit](/first-steps/pics/dji-fpv-system-air-unit-wiring-diagram-connection-f7-flight-controller-voltage-regulator-BEC.jpg?raw=true)

Воздушный модуль [Caddx Vista Air Unit](https://blog.rcdetails.info/obzor-videoperedatchik-caddx-vista-vtx-dlya-dji-digital-fpv-system/) можно использовать и с более высоким напряжением (до 6S) и, следовательно, его можно питать напрямую от 4S, без стабилизатора. Хотя для уверенности стабилизатор все же предпочтительнее.

![vista](/first-steps/pics/dji-fpv-system-air-unit-wiring-diagram-connection-caddx-vista-flight-controller-f4-vbat-lipo-voltage.jpg?raw=true)

*SBUS — подключать не обязательно.

Убедитесь, что преобразователь напряжения способен выдать необходимый ток. Ток, естественно, зависит от напряжения, макс. потребляемая мощность около 8 Вт:

- 9 вольт — 0,9 А
- 12 вольт — 0,7 А
- 16 вольт — 0,5 А

Если BEC вашего ПК не подходит по напряжению или току, то можно взять внешний преобразователь. Я использую [вот этот](https://www.banggood.com/5pcs-Mini-MP1584EN-DC-DC-BUCK-Adjustable-Step-Down-Module-4_5V-28V-Input-0_8V-20V-Output-p-1293884.html?p=AM2800122461201301GV&utm_campaign=1331474&utm_content=10344).

Прежде чем включать воздушный модуль, убедитесь, что к нему подсоединены антенны, а провода подключены согласно схеме, иначе модуль легко сжечь.

![frame](/first-steps/pics/dji-fpv-system-martian-install.jpg?raw=true)

## Привязываем очки к воздушному модулю

Чтобы получить картинку с камеры в очках, нужно привязать очки к воздушному модулю.

Включаем очки и модуль.

Берем скрепку или иголку и нажимаем кнопку привязки (link) на очках, она расположена около разъема питания. После этого вы должны услышать писк, он означает что очки готовы к привязке.

![link](/first-steps/pics/dji-fpv-system-fpv-goggles-press-link-button.jpg?raw=true)

Ждем пока светодиод на воздушном модуле не загорится зеленым, затем нажимаем кнопку (link) на нем, она расположена под слотом для MicroSD флешки.

![unit link](/first-steps/pics/dji-fpv-system-air-unit-press-link-button.jpg?raw=true)

У Caddx Vista кнопка привязки находится около USB порта (это обычная кнопка).

![vista link](/first-steps/pics/dji-fpv-system-caddx-vista-air-unit-linik-button.jpg?raw=true)

Процесс привязки занимает пару секунд. После его окончания писк в очках прекратится и появится картинка с камеры.

## Привязываем пульт управления к воздушному модулю

Если вы хотите использовать пульт от DJI для управления дроном, то его тоже нужно привязать к воздушному модулю.

Включаем модуль и пульт.

Ждем когда светодиод на модуле станет зеленым, затем нажимаем кнопку (link) на нем.

На пульте одновременно нажимаем кнопку записи, кнопку C и правую крутилку. Пульт начнет пищать.

Эта привязка тоже занимает пару секунд, после чего писк прекратится, а светодиоды на обоих устройствах будут гореть зеленым.

## Что умеет показывать Betaflight OSD до патчей

|                              | по состоянию на август 2020        |
|------------------------------|------------------------------------|
| ~~Adjustment range~~         | GPS stats                          |
| Altitude                     | GPS speed                          |
| Angle: pitch                 | Home direction                     |
| Angle: roll                  | Home distance                      |
| ~~Anti gravity~~             | ~~Link quality~~                   |
| ~~Artifical horizon~~        | ~~Motor diagnostics~~              |
| Artifical horizon sidebars   | ~~Numerical heading~~              |
| Battery average cell voltage | Numercial vario                    |
| Battery current draw         | PID pitch                          |
| Battery current mAh drawn    | PID roll                           |
| ~~Battery efficiency~~       | PID yaw                            |
| Battery usage                | Power                              |
| Battery voltage              | ~~Profile: OSD profile name~~      |
| ~~Blackbox log status~~      | Profile: PID and rate              |
| ~~Camera frame~~             | ~~Profile: PID profile name~~      |
| ~~Compass bar~~              | ~~Profile: PID rate profile name~~ |
| ~~Core temperature~~         | ~~RC Channels~~                    |
| Craft name                   | ~~RSSI dBm value~~                 |
| Crosshairs                   | RSSI value                         |
| ~~Debug~~                    | RTC date and time                  |
| Disarmed                     | ~~Stick overlay left~~             |
| ~~ESC RPM~~                  | ~~Stick overlay right~~            |
| ~~ESC RPM frequency~~        | ~~Throttle position~~              |
| ESC Temperature              | ~~Timer 1~~                        |
| ~~Flight distance~~          | ~~Timer 2~~                        |
| ~~Flip after crash arrow~~   | ~~Timer: remaining time estimate~~ |
| Fly mode                     | ~~VTX channel~~                    |
| ~~G force~~                  | ~~Warning~~                        |
| GPS latitude                 | ~~Display name~~                   |
| GPS longtitude               |                                    |