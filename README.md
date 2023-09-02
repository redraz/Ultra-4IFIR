# Ultra 4IFIR

[4IFIR Group в Телеграме](https://t.me/For4ifir)

**ВНИМАНИЕ! Автор не несет ответственности за последствия установки Ultra 4IFIR, вы все делаете на свой страх и риск.**
**Но, по моему опыту, разгон консоли абсолютно безопасен для железа консоли, но он может представлять опасность для ваших данных, портить файлы игр, сохранения или даже повредить системные файлы, поэтому крайне рекомендуется пользоваться разгоном только на Эмунанде, и всегда делать своевременные бэкапы сейвов.**

## Описание проекта
Ультимативное решение для максимального разгона и его конфигурации под вашу консоль!
Сделано на основе [4IFIR](https://github.com/rashevskyv/4IFIR), все лицензии от исходного проекта.

Включает в себя Ultra Tuner на основе [Ultrahand](https://github.com/ppkantorski/Ultrahand-Overlay)
- Позволяет настроить андервольт гпу как пакетно, переключая `ГПУ` с базы на ст или обратно, так и точечно выбрать вольтаж любой из частот.
- Возможность изменить лимит вольтажа `ЦПУ` как для эристы, так и для марико, что увеличит потолок разгона ЦПУ (Или при понижении может поправить вылеты игр)
- Выбор частоты и изменение вольтажей `РАМ`.

## Установка

1. Распакуйте архив [AIO](https://github.com/redraz/Ultra-4ifir/raw/main/AIO/AIO.zip) в корень SD карты с заменой/слиянием файлов.
2. Открываем `hb menu` (Через запуск игры с зажатой R), запускаем `All-in-One Switch Updater`, спускаемся в пункт `Сторонние загрузки`.
3. Сначала, на всякий случай выбираем `Refresh AIO`, на вопрос отвечаем `yes`, это обновит ссылки в AIO.
4. Опять заходим в `Сторонние загрузки`, выбираем `Ultra 4IFIR`, на вопрос отвечаем `yes`.

### Чистая установка
Если у вас возникли проблемы с установкой через `AIO`, то можно произвести чистую установку:
- Удаляем с карты памяти всё, кроме папок `Nintendo` и `emuMMC`, а потом распаковываем архив [Ultra 4IFIR](https://github.com/redraz/Ultra-4ifir/releases/latest/download/Ultra.4IFIR.zip) на карту.
- Это удалит все моды для игр и хоумбрю программы, но не затронет ваши игры и сохранения.


## Использование
**Для смены стейджей/настройки**
1. Открываем тесла-меню (L+R+вверх) - вместо него теперь `Ultrahand`, нажимаем вправо для перехода к плагинам. Заходим в `Ultra Tuner`, выбираем свою консоль, `Mariko` или `Erista`, и нажимаем B.
2. Так будет происходить вся дальнейшая настройка: заходим в нужный вам пункт меню, выбираем нужную настройку и нажимаем B для выхода назад. Пункты меню в это время обновляются, и на главной странице появляются новые меню.
3. Заходим в `Ultra Tuner` снова, он обновился и нам доступны новые пункты. ~~Выбираем `Initialization` - `Initial Placebo`, и снова выходим назад, пару раз нажимая B.~~ Теперь сразу переходим к следующим пунктам.
4. Теперь вы вольны настраивать систему как вам угодно, или выбрать из списка предложенных пресетов, будь то пресеты от Кулера, или от меня.
5. После конца настройки, заходим обратно в `Ultra Tuner` и выбираем `Tuning` - `Complete Tuning`, это очистит лишние пункты меню и перезагрузит консоль.
6. Если вы переборщили с разгоном/стейджем, и у вас не загружается консоль - просто войдите в `Hekate`, и выберите загрузку в `Safe Mode`, в отличии от `Semi Stock` в "безопасном режиме" не подгружается loader.kip разгона, так что можно без проблем в него загрузиться и восстановить бэкап/поставить базовый стейдж.

### Описание пресетов
В скобочках значения для Эристы
Указана реальная частота рам, при использовании будет отображаться на 200МГц выше

***Официальные от Кулера - Base<ST9<ST9+***
- Base - `РАМ` 2300мгц (1996), GPU Base,
тайминги 135652, DVB 02
   - вольтажи: cpu-1180mV (1270), vddq-640mV, vdd2-1300mV
- ST9 - `РАМ` 2400мгц (1996), GPU Stage,
тайминги 355653, DVB 00
   - вольтажи: cpu-1180mV (1270), vddq-600mV, vdd2-1275mV
- ST9+ - `РАМ` 2500мгц (2131), GPU Stage,
тайминги 555663, DVB 01
   - вольтажи: cpu-1235mV (1300), vddq-630mV, vdd2-1250mV

***Кастомные от Меня - Core<Mega<Ultra***
- Core - `РАМ` 2300мгц (1996), GPU Base,
тайминги 225652, DVB 01
   - вольтажи: cpu-1160mV (1235), vddq-650mV, vdd2-1300mV
- Mega - `РАМ` 2400мгц (2131), GPU Stage,
тайминги 455653 (525653), DVB 01
   - вольтажи: cpu-1200mV (1270), vddq-650mV, vdd2-1300mV
- Ultra - `РАМ` 2500мгц (2188), GPU Stage,
тайминги 555653 (525653), DVB 01
   - вольтажи: cpu-1220mV (1320), vddq-650mV, vdd2-1300mV
- Red - `РАМ` 2515мгц (2286), GPU Stage,
тайминги 555653 (626663), DVB 00
   - вольтажи: cpu-1220mV (1270), vddq-630mV, vdd2-1225mV (1300)

***Тестовые - для теста рам***
- Test timings - `РАМ` 2131мгц (1862), GPU Overvolt,
тайминги 555653 (626663), DVB 02
   - вольтажи: cpu-1160mV (1235), vddq-700mV, vdd2-1350mV
- Test MHz Ram - `РАМ` 2500мгц (2188), GPU Overvolt,
тайминги 111110, DVB 02
   - вольтажи: cpu-1160mV (1235), vddq-700mV, vdd2-1350mV

### Дополнение

Теперь `4ifir Micro` вшит в сам `Ultra Tuner` - достаточно распаковать архив [AIO](https://github.com/redraz/Ultra-4ifir/raw/main/AIO/AIO.zip), установить через него Тюнер + Апдейтер, перезагрузить консоль и выбрать Эристу или Марико в тюнере. После этого можно либо перезагрузиться и у вас будет база чифира, либо провести инициализацию стейджа. После этого, разгон от Чифира будет работать на Кефире/ОС Сьюте.

В `Ultra Updater` так же возможна установка разных Hombrew-приложений, как из состава оригинального 4ifir, так и других, а так же доступны моды созданные самим Кулером.


## Благодарность

Если вам понравились результаты моих стараний, и у вас появилось желание закинуть мне на шаву (или на аксессуары для свитча), то буду очень благодарен.
Сбер: 2202200513345833
