
<div id="badges" align="center">
  <h1>
  Mobile testing
  </h1>
</div>  

<div id="badges" align="center"> 
  <img src="https://oaksys.net/wp-content/uploads/2018/08/Oaksys-Mobile-Application-Testing.jpg" width="100"/>
</div>  


___
# Мобильные приложения делятся на: 
<div id="badges" align="left"> 
  <img src="https://bugza.info/wp-content/uploads/85dd607cf0dee94944c2a88d5bbe5951132448df.png" width="200"/>
</div>  

## Нативные приложения:
написаны на родном для определенной платформы языке программирования. Для Android этим языком является Kotlin/Java, для iOS - objective-С или Swift. 
Нативные приложения находятся на самом устройстве, доступ к ним можно получить, нажав на иконку. 
Устанавливаются через магазин приложений (Play Market на Android, App Store на iOS и др.).
Разработаны специально для конкретной платформы и могут использовать все возможности устройства - камеру, уведомления и т.п. (при наличии разрешений). <br/>
В зависимости от предназначения нативного приложения, оно может всецело или частично обходиться без наличия интернет-соединения. 
Нативные приложения дорогие в разоаботке и требут больших затрат на техническое обслуживание;

## Веб-приложения:
на самом деле не являются приложениями как таковыми. В сущности -это сайты, которые адаптированы и оптимизированы под любой смартфон и выглядят похоже на нативное приложение. И для того, чтобы воспользоваться им, достаточно иметь на устройстве браузер, знать адрес и располагать интернет-соединением. <br/>
Запуская мобильные веб-приложения, пользователь выполняет все те действия, которые он выполняет при переходе на любой веб-сайт, а также получает возможность «установить» их на свой рабочий стол, создав закладку страницы веб-сайта. Веб-приложения отличаются кроссплатформенностью, то есть способны функционировать, независимо от платформы девайса. <br/>
Недостатком такого вида приложений является утрата работоспособности при потере интернет-соединения. Их производительность находится на среднем уровне, в сравнении с другими видами приложений и зависит от возможностей интернет-соединения провайдера услуг. Помимо вышеперечисленного, веб-приложения не могут получить доступ к функциям системы и самого устройства;

## Гибридные приложения: 
это веб-приложение в обертке нативного приложения, что служит контейнером для отображения веб-приложения через встроенный упрощенный браузер (<a name="web"></a> webview в Android(Chrome webview в последней версии) и WKWebView в iOS). Нативный “фундамент” даёт преимущества нативных приложений: доступ к функционалу смартфона (API системы, пуши и т.п.), размещение в маркетах, иконка на рабочем столе и т.п., а сторона веб-приложений дает плюсы в виде кроссплатформенности и простоты обновления контента. Но оно работает не так быстро, как нативное приложение и графика менее адаптирована к ОС в сравнении с нативным приложением.;


# Чек- лист мобильного тестирования: 
<div id="badges" align="left"> 
  <img src="http://app-global.ru/blog/wp-content/uploads/2015/12/chek-list_po_razrabotke_mobilnih_prilozheniy.jpg" width="100"/>
</div>  


- [Функциональное тестирование](#functional)
- [Тестирование совместимости](#сompatibility)
- [Тестирование безопасности](#security)
- [Тестирование глобализации](#globalization)
- [Тестирование удобства использования](#convenience)
- [Стрессовое тестирование](#stress)
- [Кросс-платформенное тестирование](#сross-platform)
- [Тестирование производительности](#performance)


## <a name="functional"></a>  Функциональное тестирование
1. Проверка корректности установки/обновления/накатки версий
2. Запуск и отображение Splash Screen (экран-заставка).
3. Проверка работоспособности функционала 
  - регистрация(по номеру телефона/e-mail/через соц. сети) 
  - авторизация(по номеру телефона/e-mail/через соц. сети) 
  - навигация между разделами приложения
  - валидация обязательных полей
  - редактированиеданных в профиле пользователя
  - онбординг (вовлечение, удержание, покорение пользованиетя )
  - тестирование фильтров
  - функция оплаты
  - бонусы
4. Корректное отображение ошибок.
5. Работа с файлами(отправка/получение/просмотр)
6. Тестирование заглушек
  - нет товара
  - нет интернета
7. Тестирование pop-up, алертов(предупреждение об опасности)
8. Тестирование Push-уведомлений.
9. Тестирование [WebVier](#web)
10. Скролл/свайп элементов
11. Пагинация страниц
12. Ориентация экрана(книжная/альбомная)
13. Темная/светлая тема
14. Сворачивание/разворацивание приложения
15. Работа при разных типах подключения к Сети
  - 2G/ 3G/ 4G/ Wi-Fi
16. Работа в фоновом режиме


## <a name="сompatibility"></a>  Тестирование совместимости
Проверяется корректности работы программного продукта на разных версиях ОС, совместимость с различными оболичками и сторонними сервисами. <br/>
Включает:
1. Корректность работы датчиков (освещенности, температуры устройства, гироскои и др.)
2. Тестирование прерываний 
  - Входящие/исходящие звонки
  - Входящие/исходящие SMS
  - PUSH уведомления
  - Будильник
  - Режим "Не беспокоить"
 
3. Подключение внешних устройств (наушники, картой памяти)
4. Различные способы оплаты 
  - Apple Pay
  - Google Pay
5. Корректное отображение геолокации

## <a name="security"></a> Тестирование безопасности
1. Тестирование разрешений к ресурсам устройства
  - доступ к камере
  - доступ к микрофону
  - доступ к галерее
  - доступ к геолокации
3. Личные данные пользователя передаются по зашифрованным каналам.
4. Поля с личными данными скрыты астерисками

## <a name="globalization"></a>  Тестирование глобализации
**Globalization = Internationalization + Localization** <br/>
Тестирование заключается в том, чтобы проверить корректность работы приложения в разных странах и регионах, с различными форматами дат, чисел и валют.<br/>
Включает:
1. Параметры шрифта пользовательского интерфейса
2. Ввод текста в разных локализациях
3. RTL-языки (арабский, иврит, персидский) или вертикальные (восточно-азиатский, монгольский)
4. Перевод сокращений или аббревиатур
5. Корректное отображение форматов дат и времени
  - США мм / дд / гггг 
  - Европа - дд / мм / гггг
  - Канада принимает как дд / мм / гггг, так и мм / дд / гггг
  - 24-часовая нотация/12-часовая нотация
6. Соответствие мер исчисления, валюты
  - INR, индийская рупия, Индия
  - KZT, тенге, Казахстан
  - CAD, канадский доллар, Канада
  - CNY, юань жэньминьби, Китай
  - Фут(единица длины), Великобритания, США
  - Галлон аргентинский(единица объема), Аргентина
7. Формат номера телефона, адреса и почтового индекса
  - Японский порядок адресов - это почтовый индекс, штат, город
  - Английский порядок адресов - это имя, город, штат, почтовый индекс 
  - длина и формат телефонного номера 


## <a name="convenience"></a>  Тестирование удобства использования
1. Проверка выравнивания всех полей
2. Проверка на различном разрешении
  - 640 × 480
  - 800 × 600
  - 1024 × 768
  - 1280 × 800
  - 1366 × 768
  -	1400 × 900
  -	1680 × 1050
3. Проверка на различном размере экрана
4. Все шрифты соответствуют требованиям
5. Тестирование корректности отображения элементов.
6. Проверка на отсутствие грамматических и орфоргафических ошибок в тексте и сообщениях об ошибках
7. Присутствие указателей и подсказок (placeholder).
8. Проверка ссылок.
9. Тестирование анимаций и переходов.
10. Неактивные элементы отображаются серым
11. Поддержка основных жестов
12. Проверка удобства и логичности расположение блоков с контентом
13. Pixel Perfect -способ вёрстки строго по макету, при котором размеры и интервалы из макета соблюдаются с точностью до нескольких пикселей

## <a name="stress"></a>  Стрессовое тестирование
Вуцентральный процессор.
Работу в условиях нехватки памяти.
Влияние на аккумулятор.
Пропускную способность сети.

## <a name="сross-platform"></a>  Кросс-платформенное тестирование
1. Анализ работы приложения на уровне исполняемой среды.
2. Обнаружение дефектов, связанных с пользовательским окружением.

## <a name="performance"></a> Тестирование производительности
Тестирование времени загрузки.
Проверка скорости обработки запросов.
Проверка кэширования данных.
Измерение потребления ресурсов.
