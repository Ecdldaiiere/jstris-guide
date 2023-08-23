# Руководство Jstris 

Добро пожаловать в Jstris, простую головоломку с онлайн мультиплеером. Jstris известен своей скоростью и привлекает к себе талантливых игроков со всего света. Данное руководство расскажет вам в общих чертах об этой игре.

- - -

**Содержание**

- [Обзор](#обзор)
- [Управление](#управление)
- [Против игроков](#против-игроков)
  - [Default Room](#default-room)
  - [Bot Room](#bot-room)
  - [1v1 Room](#1v1-room)
  - [Slow Room](#slow-room)
  - [Map Room](#map-room)
- [Одиночная игра](#одиночная-игра)
  - [Спринт](#спринт)
  - [Очистка](#очистка)
  - [Ультра](#ультра)
  - [Выживание](#выживание)
  - [Карты](#карты)
  - [20TSD](#20tsd)
- [Настройка](#настройка)
  - [Таблицы атаки и комбо](#таблицы-атаки-и-комбо)
  - [Метод атаки](#метод-атаки)
  - [Блокировка мусора](#блокировка-мусора)
  - [Тип фигур](#тип-фигур)
  - [Рандомайзер](#рандомайзер)
  - [Длина очереди](#длина-очереди)
  - [Заполнять постоянным мусором](#заполнять-постоянным-мусором)
  - [Задержка перед фиксацией](#задержка-перед-фиксацией)
  - [Задержка очистки](#задержка-очистки)
  - [Гравитация](#гравитация)
  - [Задержка мусора](#задержка-мусора)
  - [Разброс мусора](#разброс-мусора)
  - [Шаблоны правил](#шаблоны-правил)
  - [Режим](#режим)
- [Часто задаваемые вопросы](#часто-задаваемые-вопросы)
  - [В: Могу ли я добавить бота в мою комнату?](#в-могу-ли-я-добавить-бота-в-мою-комнату)
  - [В: Что означают сокращения в таблице результатов игры?](#в-что-означают-сокращения-в-таблице-результатов-игры)
  - [В: Что такое DAS?](#в-что-такое-das)
  - [В: Что такое ARR?](#в-что-такое-arr)
  - [В: Что такое техника?](#в-что-такое-техника)
  - [В: Могу ли я создать приватную комнату?](#в-могу-ли-я-создать-приватную-комнату)
  - [В: Могу ли я играть в Jstris офлайн?](#в-могу-ли-я-играть-в-jstris-офлайн)
- [Дополнительная информация](#дополнительная-информация)

- - -

## Обзор 

Jstris использует те же самые базовые механики, как и большинство похожих игр. Одной из основных особенностей является обширное использование повторов. Для каждой законченной вами игры будет создан повтор. Просмотр и анализ своих игр является неотъемлемой частью самосовершенствования, и повторы Jstris предоставляют вам такую возможность.

В отличии от других игр, вы можете быть уверены, что лидеры Jstris абсолютно чисты и не используют читы. Модераторы удаляют подозрительные записи, чтобы гарантировать заслуживающий доверия список глобальных достижений.

Можно играть без регистрации, но для того, чтобы получить доступ ко всем возможностям сайта, рекомендуется создать аккаунт. Для этого, выберите пункт *Зарегистрироваться* в верхнем правом углу. Необходимы только email, имя пользователя и пароль. С аккаунтом, вы можете видеть множество статистики, включая ваши лучшие рекорды в одиночных режимах, статистику мультиплеера, статистику улучшения, повторы и многое другое. Вы также можете видеть себя в списке глобальных достижений (анонимные достижения не показаны).

![Обзор][image2]
- - -

## Управление

Jstris позволяет игрокам настроить своё управление в любое время в меню **Настройки**, которое расположено под игровым полем. Управление по умолчанию представлено ниже:

|      Команда      | Клавиша по умолчанию |
| ----------------- | -------------------- |
| Налево            | left                 |
| Направо           | right                |
| Мягкое падение    | down                 |
| Быстрое падение   | space                |
| Поворот налево    | z                    |
| Поворот направо   | up                   |
| Переворот         | a                    |
| Замена            | c                    |

## Против игроков

### Default Room

При входе на сайт, все игроки изначально попадают в **Default room** - комнату со свободным доступом, где можно встретить игроков любого уровня.

Игра в комнате по умолчанию может быть тяжелой. Уникальной особенностью Jstris является то, что он смешивает скромных новичков с мировыми топ игроками, и всеми остальными. Если вы устали играть и хотите просто наблюдать, используйте команду  `/spectate` или `/spec`. Чтобы вернуться к игре, используйте `/play`.

### Bot Room

Default Room не единственная доступная комната. Чтобы увидеть весь список, нажмите кнопку *Лобби* под игровым полем. Следующей по популярности комнатой является комната с ботами **Bot Room**, названная так, потому что в ней всегда присутствует бот. Вы можете узнать его по красному цвету, он находится среди других оппонентов в левом верхнем углу.

![Бот MisaMino среди оппонентов][image4]

В Jstris 4 вида ботов. В списке ниже они отсортированы по силе, также представлены команды для смены бота.

- MisaMino: `/changeBot misamino`
- Real_Block: `/changeBot real`
- ~~jez_Block: `/changeBot jez`~~ (удалён 2018.09.21)
- ~~Fool bot: `/changeBot fool`~~ (удалён 2018.09.21)

*\*Любые команды должны быть введены между играми. Всякая команда, введённая во время игры, игнорируется.*

Misamino - самый сильный бот, возможно, сильнейший среди когда-либо созданных ботов. На его максимальной скорости 5 PPS (фигур в секунду), он становится грозным оппонентом, который может легко победить самых сильных живых игроков в режиме 1 на 1. Однако, производительности бота не хватает когда в комнате больше 5 живых игроков, и обычно он сразу же проигрывает. Для настройки бота можно использовать команду /botPPS.

Скорость бота может быть изменена. Для этого, введите `/bot ?` , где замените знак вопроса на любое число между .3 и 5. Для примера, если я хочу чтобы бот играл на 2 PPS, я напечатаю `/bot 2`. Если я хочу, чтобы бот играл на 1.73 PPS, я напечатаю `/bot 1.73`.

### 1v1 Room

Комната **1v1 Room** позволяет играть только двоим игрокам, хотя кто угодно может войти и смотреть матч, даже если комната заполнена. Используйте эту комнату для игры с друзьями или с достойным оппонентом. Для того, чтобы сбросить счёт побед, используйте команду `/resetCounter` и все победы будут обнулены.

### Slow Room

Хотите сыграть с другом, но один из вас играет значительно лучше другого? Или вы просто новичок и устали мгновенно проигрывать в комнатах с про-игроками? Или вы хотите улучшить эффективность своей игры, убрав скорость из общего зачёта? В Jstris есть Slow Room (медленная комната) для всех этих случаев. По умолчанию скорость медленной комнаты ограничена 2.0 PPS, что означает игроки не могут превысить этот порог. При попытке сыграть быстрее, экран будет временно заблокирован. В дополнение к ограничению скороcти, медленная комната имеет задержку 500 мс при очистке линий. Это означает что при каждой очистке вы будете ждать 500 мс, прежде чем можно будет делать что-либо ещё. Все медленные комнаты обозначаются значком спидометра - [SPEEDOMETER_ICON]. Медленные комнаты могут иметь ограничение от 0 до 20 PPS.

![Лобби, в котором вы можете создавать комнаты и присоединяться к ним][image5]

### Map Room

**Map Room** - это место, где можно соревноваться в очистке на случайной пользовательской карте. Число (D=?%), показываемое рядом с именем карты, означает сложность карты, где 0% - легчайшая карта, и 100% - сложнейшая. Карты, требующие завершения с Perfect Clear, не выпадают в этой комнате.

- - -

## Одиночная игра

### Спринт

Базовый режим с простейшей целью, **Спринт** - самый популярный режим одиночной игры в Jstris. Очистите Х линий так быстро, как можете. В Jstris есть спринт режимы для 20, 40, 100 и 1000 линий.

### Очистка

Не такой быстрый, и более аналитический, чем Спринт, режим **Очистки** предполагает больше размышлений в процессе очищения мусора наиболее эффективным способом. В Jstris есть режимы очистки для 10, 18, 100 и бесконечного числа линий.

### Ультра

Режим, рассчитанный на набор максимального количество очков, и награждающий за продвинутые техники, такие, как T-спины и back-to-back. **Ультра** - замечательный способ тренировать атаку для последующего применения в режимах против игроков.

### Выживание

Возможно, самый сложный режим среди всех режимов одиночной игры. **Выживание** похож на очистку, но мусор добавляется с постоянной скоростью: 1 линия в секунду. Выживайте против растущих линий так долго, как можете.

### Карты

Режим **Карты** был добавлен в Jstris в конце 2018 года. Карты вносят элемент креативности, при этом улучшая навыки очистки в сложных и необычных позициях. Создайте свою карту в **Дизайнере Карт**. Как только карта опубликована, игроки из любой точки мира могут играть и соревноваться в скорости на вашей карте. В Jstris ограничивает создание карт пятью публикациями в день и десятью неопубликованными картами в очереди. Карты включены в список рекордов. На каждой карте можно завоевать три медали: золотую за первое, серебряную за второе, бронзовую за третье место. Пробуйте войти в топ-3 на любой карте чтобы завоевать медали и своё место в таблице лидеров!

*\*Таблица лидеров карт обновляется несколько раз в день, поэтому изменения в ней не мгновенно отражают текущую ситуацию.*

### 20TSD

Цель этого режима - выполнить как можно больше TSD (T-spin Double) друг за другом. Если вы очищаете линию, не используя TSD, игра завершается. Режим назван 20TSD, потому что изначально люди выполняли спринт длиной 40 линий, используя только TSD (20 х 2 = 40). Однако, многие игроки выходят за эти рамки и регулярно превышают число 20.

- - -

## Настройка

Чтобы увидеть настройки любой комнаты, используйте команду `/config`. Ниже мы пробежимся по возможным опциям.

### Таблицы атаки и комбо

По умолчанию, атака и комбо в Jstris выглядят так (можно перенастроить в приватных комнатах):

| Тип атаки          | Кол-во посланных линий |   | Комбо # | Кол-во посланных линий |
| :----------------- | ---------------------: | - | ------: | ---------------------: |
| 1 линия (single)   |                  **0** |   |       1 |                  **0** |
| 2 линии (double)   |                  **1** |   |       2 |                  **1** |
| 3 линии (triple)   |                  **2** |   |       3 |                  **1** |
| 4 линии            |                  **4** |   |       4 |                  **1** |
| T-spin Double      |                  **4** |   |       5 |                  **2** |
| T-spin Triple      |                  **6** |   |       6 |                  **2** |
| T-spin Single      |                  **2** |   |       7 |                  **3** |
| T-spin Mini Single |                  **0** |   |       8 |                  **3** |
| Perfect Clear      |                 **10** |   |       9 |                  **4** |
| Back-to-Back       |                 **+1** |   |      10 |                  **4** |
|                    |                        |   |      11 |                  **4** |
|                    |                        |   |     12+ |                  **5** |

### Метод атаки

В Jstris существует 8 опций для распределения мусора от вашей атаки в матчах против игроков:

- Targets (Прицел) `/set garbage targets`
- Divide (Разделение) `/set garbage divide`
- To all (Всем) `/set garbage toAll`
- To least (По меньшинству) `/set garbage toLeast`
- To most (Сильнейшему) `/set garbage toMost`
- To self (Себе) `/set garbage toSelf`
- Random (Случайно) `/set garbage random`
- Roulette (Рулетка) `/set garbage roulette`

**Targets** (Прицел) - обычно является опцией по умолчанию и самым популярным выбором. В этом режиме, цель равновероятно выбирается по очереди из всех оппонентов в комнате. Игрок, являющийся целью в момент атаки, получает посланный вами мусор.

**Divide** (Разделение) - мусор делится поровну между игроками комнаты. Например, если вы выполняете TSD в комнате с двумя другими оппонентами, каждый из них получит по 2 линии мусора.

**To all** (Всем) - все производимые вами атаки отсылаются каждому из ваших оппонентов в комнате. К примеру, если вы выполняете Perfect Clear в комнате с 4-мя оппонентами, то каждый из них получает 10 линий мусора, то есть, вы посылаете 40 линий мусора в целом. Из приведённого примера вы уже наверное поняли, что игры в этом режиме с беспорядочно возрастающим мусором характерно короткие.

**To least** (По меньшинству) - мусор получает игрок, который *пострадал* меньше всех от предыдущих атак. Предположим, в комнате с тремя оппонентами, вы посылаете 4 линии. Игрок А уже получил 50 линий урона к этому моменту. Игрок Б получил 53. Игрок В получил 58. Так, как игрок А получил меньше всего линий, вся ваша атака - 4 линии, отправляется к нему.

**To most** (Сильнейшему) - мусор получает игрок, которые *послал* больше всего атак. По сути, вы атакуете самого сильного игрока комнаты.

**To self** (Себе) - ваша атака отсылается вам самому. Непрактично в игре против других игроков, но кому-то этот режим может быть полезен для тренировок в одиночку.

**Random** (Случайно) - атака отсылается случайному оппоненту. Возможно, самый честный режим.

**Roulette** (Рулетка) - тоже самое, что предыдущее, но атака может быть послана и вам в том числе.

### Блокировка мусора 

В Jstris 4 типа блокировки мусора:

- Full (Полная)
- Limited (Ограниченная)
- None (Отсутствует)
- Instant (Мгновенная)

**Full** (Полная) - блокировка по умолчанию. Другие игры, которые используют Full, это *TF* (комнаты e+) и *TOP*.  В этом режиме, появляется индикатор мусора в виде красной полосы справа от вашего игрового поля. Мусор не попадает на ваше поле до тех пор, пока вы не поставите блок. Мусор может быть уменьшен с помощью вашей атаки (например, снятием 4-х линий). Если вы начали комбо, то мусор будет заморожен от появления на поле до тех пор, пока вы не закончите своё комбо.

**Limited** (Ограниченная) - данный тип блокировки очень похож на Full, но с одним отличием. Входящий мусор попадает на ваше поле вне зависимости от того, выполняете ли вы комбо или нет. Другими словами, мусор не приостанавливается во время комб, как в режиме Full. Входящий мусор также может быть уменьшен с помощью атак. Игры, использующие Limited включают *PPT*, *TB* и *TF* (не e+ комнаты).

**None** (Отсутствует) - в этом режиме, мусор не может быть уменьшен или отменён. Изначально он появляется в виде красной полосы (как в режимах Full и Limited), и попадает на ваше игровое поле как только вы поставите блок. К примеру, если оппонент послал вам 10 линий, даже если вы сняли 4 линии следующим блоком, то входящий мусор не будет уменьшен до 6 линий. Вместо этого, вы получите все 10 линий мусора, и пошлёте оппоненту 4 линии.

**Instant** (Мгновенная) - в этом режиме вообще нет красной полосы. Мусор попадает на ваше поле в момент, когда оппонент посылает его. Отмена части мусора невозможна.

|         | Красная полоса | Отмена |
| ------- | :------------: | :----: |
| Full    |       Да       |  Да    |
| Limited |       Да       |  Да    |
| None    |       Да       |  Нет   |
| Instant |       Нет      |  Нет   |

### Тип фигур

В игре 8 типов наборов фигур.

- Standard
- Big
- ARS
- Penta
- M123
- All-29
- C2RS
- O-spin

**Standard** Самые распространённые и простые тетромино, с которыми вы уже вероятно знакомы. Являются блоками по умолчанию.

**Big** Увеличенные в 4 раза по сравнению со стандартными блоками, такие блоки наносят массивный урон.

**ARS** Стандартные блоки, но управляемые ARS (Arika rotation system), включая CC-проверку. Запрограммированы NueSB

**Penta** Пентамино блоки, 18 разных фигур.

**M123** Блоки размером 1,2 и 3. Всего существует 4 разных блоков такого типа.

**All-29** Блоки размером 1,2,3,4,5, всего 29 разных блоков. Включает в себя 7 стандартных, 4 M123 и 18 пентаблоков.

**C2RS** стандартные блоки, но управляемые Cultris 2 rotation system.

**O-spin** система поворотов, возникшая из мемов, где возможны тройной (2 х по часовой стрелке) и четверной (1 х против часовой стрелки) повороты фигуры О. Также, возможны другие нетрадиционные повороты (из за того, что таблица толчков содержит 15 уровней, тогда как стандартная система поворотов SRS содержит только 4 уровня).

### Рандомайзер

Рандомайзер - это формула, по которой формируется порядок выпадающих блоков. Jstris имеет 11 разных рандомайзеров:

- 7-bag
- 14-bag
- Classic
- C2Sim
- One block
- Two block
- One 7-bag
- One 14-bag
- Repeat+7b
- BSblock+7b
- BigBlock+7b

**7-bag** - стандартный рандомайзер по умолчанию. Представьте себе мешок с 7-ю фигурами, по одной из всех возможных. Вы вытаскиваете из мешка фигуры одну за одной, до тех пор, пока он не опустеет. Тогда вы получаете точно такой же новый мешок, опять с 7-ю фигурами. Опять вытаскиваете одну за одной до тех пор, пока он не опустеет. Повторяете. Так и работает 7-bag рандомайзер.

**14-bag** - похож на 7-bag, но двойного размера, с двумя фигурами каждого типа из 7-ми возможных блоков. Также вытаскиваете по одной фигуре до тех пор, пока мешок не опустеет. Повторяете.

**Classic** - полностью случайные фигуры. Этот рандомайзер делает постройку очень трудным делом.

**C2Sim** - рандомайзер Cultris 2, описанный здесь [post by Integration](http://harddrop.com/forums/index.php?showtopic=5080&st=0&p=71443&#entry71443)

**One block** - этот рандомайзер даёт вам только одну фигуру, выбранную случайно в начале игры. Вам будет выпадать только этот блок.

**Two block** - рандомайзер, похожий на предыдущий, но дающий два разных блока вместо одного.

**One 7-bag** - первый мешок в игре будет повторяться бесконечно. Используя этот рандомайзер, одна и та же очередь из 7 фигур будет выпадать снова и снова.

**One 14-bag** - похоже на предыдущий режим, но очередь ограничена 14-ю фигурами, которые будут повторяться снова и снова.

**Repeat+7b** - работает, как 7-bag, только каждая фигура в мешке имеет шанс быть повторённой 1-7 раз.

**BSblock+7b** - работает, как 7-bag, только может включать фигуры из других наборов блоков, например, пентамино или больших блоков.

**BigBlock+7b** - работает, как 7-bag, только может включать большие блоки.

### Длина очереди 

Jstris по умолчанию показывает 5 превью очереди. В созданных вами комнатах, вы можете настроить от нуля до пяти превью.

### Заполнять постоянным мусором

Постоянный мусор это неочищаемые линии, которые прибавляются снизу для того, чтобы подогнать игру и она не продолжалась бесконечно. Такие линии немного темнее, чем обычный мусор. В комнате Bot Room постоянный мусор по умолчанию начинает появляться через 2 минуты. Этот параметр можно настроить в созданных вами комнатах.

![Solid Garbage][image7]

### Задержка перед фиксацией

Задержка перед фиксацией означает сколько времени установленная фигура будет ожидать прежде чем зафиксируется. В Jstris есть три типа задержек, которые можно настроить. Первая, L1, означает задержку перед фиксацией фигуры после мягкого падения. По умолчанию, задержка L1 = 500 мс. Вторая, L2, означает как долго можно перемещать уроненную мягким падением фигуру налево или направо (по умолчанию 5000 мс). Следует заметить, что если фигуру повернули, то L2 сбрасывается и фигура может быть перемещена дольше, чем в течении обычных 5000 мс, что приводит нас к задержке L3. L3 означает максимальное количество времени после появления фигуры на поле, перед её финальной фиксацией, вне зависимости от совершаемых вами действий. По умолчанию, L3 = 20000 мс.

### Задержка очистки

Задержка очистки это фиксированное количество времени, которое проходит после очистки одной или более линий. Во время этой задержки вы не можете ничего делать. Много классических пазловых игр и PPT используют задержку очистки, но в Jstris по умолчанию задержка очистки = 0, и для большинства режимов она никогда не используется. Однако, это настраивается, если вы хотите включить её. Допустимые значения - от нуля и до 6000 мс.

### Гравитация

Гравитация представляет собой скорость, с которой фигуры автоматически падают вниз. Гравитация может быть изменена в пределах 0-28 уровня. Гравитация по умолчанию = 1. Если гравитация = 0, то фигура не упадёт вниз до тех пор, пока не истечёт задержка L3 (по умолчанию, 20 секунд). 28 уровень гравитации эквивалентен 20G, при этом фигура мгновенно падает до самого низа.

### Задержка мусора

Задержка мусора это фиксированное количество времени между тем, как входящий мусор появляется на красной полосе и его появлением на игровом поле. По умолчанию она равна 500 мс. Данный параметр настраивается в пределах от 0 до 60000 мс. Более высокая задержка позволяет отыграть большее количество блоков, прежде чем мусор будет помещён на поле; более низкая задержка способствует меньшему количеству. Другими словами, чем больше задержка, тем больше возможностей для блокирования мусора. Другой способ определить задержку мусора - "минимальное количество времени после входящей атаки, когда мусор будет отображен красной полосой, и прежде чем он попадёт на игровое поле".

### Разброс мусора

Разброс мусора отражает его сложность для очистки вами. Чтобы изменить разброс, используйте команду `/set messiness ?`, где ? заменён на любое число от -100 до 100. -100 - наилегчайшая опция, отверстия на протяжении всего слоя мусора будут находиться друг над другом (левая картинка). 100 - наисложнейшая опция, отверстия будут находиться в случайных позициях в любой из 10 колонок, делая его максимально сложным для очистки (правая картинка).

![Unmessy (-100)][image10] 
![Messy (100)][image1]

### Шаблоны правил

Если существует какой то набор правил, который вам особенно нравится и вы хотите легко выбирать его, вы можете сохранить его как шаблон.

Чтобы выполнить это, зайдите в *Лобби*, затем выберите *Создать комнату*, затем в строке *Больше правил* выберите *Простые* либо *Все*. После того, как вы настроили все параметры, нажмите кнопку *Сохранить* внизу, игра создаст вам шаблон. Скопируйте данные и воспользуйтесь формой отправки шаблона для пересылки на сервер.
[Submit a preset](/presets/submit) 

Как только вы отправили шаблон, вы можете просматривать его, наряду с другими пользовательскими шаблонами [List of presets](/presets). Теперь можно легко воссоздать те же самые правила без настройки всех опций. Просто выберите *Создать комнату*, *Использовать правила* и выберите ваш шаблон.

### Режим

В Jstris сейчас присутствует 7 режимов, среди которых вы можете выбирать при создании своей комнаты:

- Стандартный
- Командный
- Очистка
- Live Sprint
- Live Cheese
- Live Survival
- Live Maps v0.1

**Стандартный** режим это нормальный мультиплеер со свободным доступом. 

**Командный** режим создаёт командную комнату. Выбирайте сторону, красную или синюю, и принесите победу своей команде. Для выбора имени команды, используйте `/set teamName ?`, где вместо знака вопроса введите желаемое имя.

![team game in progress][image11]

**Очистка** создаёт комнату для очистки. Посылаемый вами мусор - это основной путь выиграть оппонента в режиме против игроков. Важным скиллом является очистка мусора. Практикуйтесь в очистке на скорость в режиме против игроков. Первый, добравшийся до дна в мусоре высотой 10 линий, побеждает. 10 линий слишком легко для вас? Измените высоту мусора командой `/set height ?`, где знак вопроса заменён на число от 1 до 20.

Режим **Live Sprint** позволяет вам играть спринт против оппонентов. Тот, кто завершил спринт быстрее всех, выигрывает. По умолчанию играется спринт длиной в 40 линий, но вы можете изменить это с помощью следующих команд:

- 20L:     `/set gamemode sprint20`
- 40L:     `/set gamemode sprint40`
- 100L:    `/set gamemode sprint100`
- 1000L:   `/set gamemode sprint1000`

Если вы устанавливаете личный рекорд в Live Sprint, то, к сожалению, это не будет отражено в вашем аккаунте, потому что пишется повтор против игроков, а не обычный повтор. Но вы можете добавить его в избранное, если хотите сохранить.

Режим **Live Cheese** позволяет играть в очистку против оппонентов. Этот режим точно такой же, как и режим очистки, за исключением того, что вы не можете выбирать никаких других значений для высоты мусора, кроме 10, 18 и 100 линий. По умолчанию высота равняется десяти линиям, но вы можете изменить это следующими командами:

- 10L:     `/set gamemode cheese10`
- 18L:     `/set gamemode cheese18`
- 100L:    `/set gamemode cheese100`

Режим **Live Survial** позволяет вам играть в режим Выживания против оппонентов. Кто выживет дольше всех, выигрывает.

**Live Maps v0.1** позволяет вам играть в режим Map Room против оппонентов.

## Часто задаваемые вопросы

### В: Могу ли я добавить бота в мою комнату?
О: Нет. В данный момент у нас только один бот в Jstris, который постоянно находится в Bot Room. Однако, данный функционал может быть добавлен в будущем.

### В: Что означают сокращения в таблице результатов игры?

О: B2B = back-to-back. B2Bpm = back-to-back per minute (B2B в минуту). APM = attack per minute (атак в минуту). SPM = sent per minute (послано в минуту). PPS = pieces per second (фигур в секунду). Rep = replay (повтор).

![game results table][image9]

### В: Что такое DAS?

О: DAS это мера горизонтальной чувствительности фигуры. DAS означает delayed auto shift, задержка автоповтора. Это контролирует, как долго вы должны держать клавишу влево или вправо прежде чем фигура автоматически начнёт двигаться в желаемую сторону. С низким DAS даже легчайшее касание клавиши мгновенно подвинет фигуру. С высоким DAS вы будете вынуждены держать кнопку направления дольше, прежде чем фигура начнёт движение. DAS по умолчанию в Jstris равен 133 мс. Если это кажется вам слишком чувствительным, повысьте значение. Если кажется слишком медленным, понизьте. Отрегулируйте DAS так, как вам нравится.

### В: Что такое ARR?

О: ARR это другая форма горизонтальной чувствительности фигуры. ARR означает auto repeat rate, скорость автоповтора. Это контролирует как быстро фигура двигается влево или вправо. Данный термин понять немного проще, чем DAS. С низким ARR, фигура почти мгновенно достигнет стены в той стороне, куда вы её направляете. С высоким ARR, фигура будет двигаться к стене медленно, пока вы держите кнопку направления. ARR по умолчанию равен 10 мс в Jstris.

### В: Что такое техника?

О: техника - это наиболее эффективный путь передвижения фигуры. Хорошая техника важна для того, чтобы играть ровнее и быстрее. Число рядом с этим термином означает как много ошибок техники вы совершили. Таким образом, техника 0 означает что вы не совершили ни одной технической ошибки. В идеале, чем ближе это число к нулю, тем лучше. Техника - это то, что вы должны учить чтобы использовать её правильно. Существует много ресурсов, объясняющих правильную технику. Это видео может стать хорошей стартовой точкой в изучении: [Tutorial: How to Play Fast!](https://youtu.be/_QBs703nOnk?t=502).

### В: Могу ли я создать приватную комнату?

О: Да. Выберите *Лобби*, затем *Создать комнату*, затем кликните по чекбоксу *Приватная*. Скопируйте ссылку и дайте тому, кого хотите пригласить в свою комнату. Подсказка: вы можете узнать ссылку на любую комнату, публичную или приватную с помощью команды `/link`.

### В: Могу ли я играть в Jstris оффлайн?

О: Да. Для этого скачайте Jstris пока вы онлайн. Для этого, нажмите правой кнопкой мыши по странице, выберите в меню пункт "Сохранить страницу как" и сохраните html файл. Следует заметить, что только режимы одиночной игры доступны офлайн, и ваш счёт не будет сохранён.

- - -

## Дополнительная информация

Существование Jstris полностью зависит от донатов. В игре нет рекламы. Из-за того, что игра хранит повторы и данные, Jstris нужен мощный сервер. Я благодарен всем донатам, и они будут поддерживать Jstris в рабочем состоянии. Читайте раздел [About](/about) веб сайта, чтобы узнать больше.

[image2]: ./images/guide-intro.png "introduction"
[image4]: ./images/image4.png "MisaMino bot in opponents view"
[image8]: ./images/image8.png "speedometer icon for Speed Limit Rooms"
[image5]: ./images/image5.png "the lobby, where you can join and create rooms"
[image11]: ./images/image11.png "team game in progress"
[image7]: ./images/image7.png "Solid Garbage"
[image10]: ./images/image10.png "Unmessy (-100)"
[image1]: ./images/image1.png "Messy (100)"
[image9]: ./images/image9.png "game results table"