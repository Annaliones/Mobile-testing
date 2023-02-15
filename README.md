
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
Разработаны специально для конкретной платформы и могут использовать все возможности устройства - камеру, уведомления и т.п. (при наличии разрешений). 
В зависимости от предназначения нативного приложения, оно может всецело или частично обходиться без наличия интернет-соединения. 
Нативные приложения дорогие в разоаботке и требут больших затрат на техническое обслуживание;

## Веб-приложения:
на самом деле не являются приложениями как таковыми. В сущности -это сайты, которые адаптированы и оптимизированы под любой смартфон и выглядят похоже на нативное приложение. И для того, чтобы воспользоваться им, достаточно иметь на устройстве браузер, знать адрес и располагать интернет-соединением. Запуская мобильные веб-приложения, пользователь выполняет все те действия, которые он выполняет при переходе на любой веб-сайт, а также получает возможность «установить» их на свой рабочий стол, создав закладку страницы веб-сайта. Веб-приложения отличаются кроссплатформенностью, то есть способны функционировать, независимо от платформы девайса. Недостатком такого вида приложений является утрата работоспособности при потере интернет-соединения. Их производительность находится на среднем уровне, в сравнении с другими видами приложений и зависит от возможностей интернет-соединения провайдера услуг. Помимо вышеперечисленного, веб-приложения не могут получить доступ к функциям системы и самого устройства;

## Гибридные приложения: 
это веб-приложение в обертке нативного приложения, что служит контейнером для отображения веб-приложения через встроенный упрощенный браузер (webview в Android(Chrome webview в последней версии) и WKWebView в iOS). Нативный “фундамент” даёт преимущества нативных приложений: доступ к функционалу смартфона (API системы, пуши и т.п.), размещение в маркетах, иконка на рабочем столе и т.п., а сторона веб-приложений дает плюсы в виде кроссплатформенности и простоты обновления контента. Но оно работает не так быстро, как нативное приложение и графика менее адаптирована к ОС в сравнении с нативным приложением.;


# Чек- лист мобильного тестирования: 
<div id="badges" align="left"> 
  <img src="http://app-global.ru/blog/wp-content/uploads/2015/12/chek-list_po_razrabotke_mobilnih_prilozheniy.jpg" width="100"/>
</div>  


- [Функциональное тестирование](#functional)
- [Тестирование совместимости](#сompatibility)
- [Тестирование безопасности](#security)
- [Тестирование глобализации](#Globalization)
- [Тестирование удобства использования](#convenience)
- [Стрессовое тестирование](#stress)
- [Кросс-платформенное тестирование](#сross-platform)
- [Тестирование производительности](#performance)


## <a name="functional"></a>  Функциональное тестирование



## <a name="сompatibility"></a>  Тестирование совместимости
Проверяется корректности работы программного продукта на разных версиях ОС, совместимость с различными оболичками и сторонними сервисами.
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
  - 

## <a name="security"></a> Тестирование безопасности

## <a name="Globalization"></a>  Тестирование глобализации
** Globalization = Internationalization + Localization**
Тестирование заключается в том, чтобы проверить корректность работы приложения в разных странах и регионах, с различными форматами дат, чисел и валют.
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


## <a name="convenience"></a>  Тестирование удобства использования

## <a name="stress"></a>  Стрессовое тестирование

## <a name="сross-platform"></a>  Кросс-платформенное тестирование

## <a name="performance"></a> Тестирование производительности
