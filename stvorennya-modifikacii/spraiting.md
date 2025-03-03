---
icon: aperture
---
# Спрайтинг

Спрайтинг є важливою частиною моддингу Mindustry; все, що ви створили, відображатиметься як погано масштабовані зображення "oh no" без належного спрайтингу.

Стиль спрайтингу в Mindustry простий, але дуже обмежений; те, що можна використовувати в інших іграх, виглядатиме недоречно в Mindustry.

Усі ванільні спрайти можна знайти [тут](https://github.com/Anuken/Mindustry/tree/master/core/assets-raw/sprites).

**Зверніть увагу, що використання спрайтів інших розробників модів без їхнього дозволу заборонено, хоча ви можете використовувати їх для натхнення або як довідку.**

**Аргументи на кшталт "Мод має відкритий код, я можу робити з ним все, що захочу" чи подібні не будуть визнані або толеровані, а ваш мод буде занесено в чорний список браузера модів.**

## **Програми для спрайтингу**

Наполегливо рекомендується використовувати програми для спрайтингу, які підтримують прозорість та експорт зображень у форматі `.PNG`. Нижче наведено список рекомендованих програм.

### **Десктопні програми**

    1. **[Aseprite](https://www.aseprite.org/)**

    - Золотий стандарт. Має деяку криву навчання, але дуже простий у використанні після звикання.
    - Це **платне** програмне забезпечення, але ви можете **[скомпілювати вихідний код самостійно](https://github.com/aseprite/aseprite/blob/main/INSTALL.md#compiling)**. Будь ласка, придбайте ліцензію, щоб підтримати його розробників.
      - Має багато корисних функцій для спрайтингу в стилі Mindustry, таких як:
         - Дзеркалювання
         - Керування палітрою
         - Анімація
         - Шарування (також можливість експортувати окремі шари)

    2. **[LibreSprite](https://libresprite.github.io/#!/)**
       - Форк репозиторію Aseprite, не такий актуальний чи потужний як Aseprite, але підходить для спрайтингу в стилі Mindustry.

    3. **[Piskel](https://www.piskelapp.com/)**
       - Проста програма для піксельної графіки, не така потужна як Aseprite чи LibreSprite, але цілком достатня. Існує онлайн-версія та офлайн-версія для завантаження, обидві з однаковими функціями.
       - Не підтримує експорт окремих шарів

    4. **[Pixilart](https://www.pixilart.com/)**
       - Онлайн-інструмент для спрайтингу, який має більше функцій ніж Piskel, але не має інструменту дзеркалювання. Якщо ви більш знайомі з Pixilart, використовуйте його замість Piskel.
       - Доволі громіздкий для спрайтингу в стилі Mindustry.

    5. **[Paint.NET](https://www.getpaint.net/)**
       - Дуже базовий інструмент для малювання, не плутати з Paint 3D. Paint.NET можна використовувати, але він не такий зручний, як вищезгадані програми.
       - Paint.NET не має основних функцій, необхідних для спрайтингу в стилі Mindustry. Ви можете отримати деякі з цих функцій через плагіни.
       - Але все ж не рекомендується використовувати його заради зручності. Якщо ви можете завантажити Paint.NET, ви, ймовірно, можете завантажити Piskel або LibreSprite, які призначені для піксельної графіки.

### **Мобільні програми**

1. **[Novix Pixel Editor](https://play.google.com/store/apps/details?id=io.anuke.novix)**
   - Старий і надійний, створений і покинутий Ануке, простий, без реклами, хоч і трохи застарілий, але все ще надійний інструмент для спрайтингу на мобільних пристроях, також підтримує інструмент дзеркала.
   - Іноді ламається при створенні більших спрайтів.

2. **[Pixel Studio](https://play.google.com/store/apps/details?id=com.PixelStudio)**
   - Одна з найпопулярніших програм для піксельної графіки.
   - Має більшість необхідних вам функцій і може також синхронізуватись з ПК-версією.
   - Містить рекламу

3. **[Ibispaint X](https://play.google.com/store/apps/details?id=jp.ne.ibis.ibispaintx.app)**
   - Не призначена для спрайтингу і вимагає деяких змін налаштувань перед використанням.
   - Підтримує різні інструменти, такі як октагональні дзеркала, світіння та градієнти, а також основні функції, як вибір області та шари.
   - Може використовуватися для створення складних спрайтів з легкістю, але може бути громіздкою для простих спрайтів.
   - Також містить рекламу

## **Розміри**

### Блоки

Найменший розмір спрайту блоку, який ви можете створити, це `32px × 32px`, що відповідає блоку 1×1. Створення більших блоків означає збільшення розміру спрайту на додаткові `32px`, тож блок 2×2 має розмір `64 × 64` тощо. Це стосується як турелей, так і блоків.

- `1×1` : `32px × 32px`
- `2×2` : `64px × 64px`
- `3×3` : `96px × 96px`
- `4×4` : `128px × 128px`
- `5×5` : `160px × 160px`

Ви не обмежені цими розмірами; гра все одно завантажить спрайти більші або менші за рекомендовані, що може призвести до унікального вигляду спрайту або до кошмару.

### Предмети, рідини, статуси

Для цих типів вмісту мінімальний розмір спрайту становить `32px`; ви можете використовувати більші зображення, але гра стисне їх до `32px`. Гра не збільшить менші зображення, тому `32px` є мінімальним розміром.

### Юніти

Розміри спрайтів юнітів більш гнучкі ніж для інших типів, хоча намагайтеся не опускатися нижче `48px`. Чим більші ваші юніти, тим більше вам доведеться коригувати їх `hitSize` (розмір хітбоксу).

## **Зберігання спрайтів**

Спрайти можуть бути поміщені в піддиректорію `sprites/` вашого мода, якщо це hJSON, або `src/assets/sprites/`, якщо це мод на Java. Парсер контенту рекурсивно шукатиме їх.

Зображення пакуються в "атлас" для ефективного рендерингу. Перша директорія в sprites/, наприклад, `sprites/blocks`, визначає сторінку в цьому атласі, куди поміщаються спрайти. Розміщення спрайту блоку в папці юнітів може спричинити значні затримки; тому вам слід намагатися організовувати все подібно до того, як це робить ванільна гра.

Гра шукатиме спрайти для контенту на основі його назви. `content/blocks/test-turret.json` має назву `test-turret`, і аналогічно, `sprites/test-turret.png` має назву `test-turret`, тому він буде використовуватися цим контентом.

- Блоки повинні зберігатися в `sprites/blocks`
- Юніти повинні зберігатися в `sprites/units`
- Предмети повинні зберігатися в `sprites/items`

Гра модифікуватиме деякі спрайти. До турелей та юнітів буде додано сіру рамку товщиною `3-4px`, тому ви повинні враховувати це під час створення спрайтів, залишаючи простір навколо турелей. Стандартний радіус контуру та колір можна налаштувати, змінивши поля `outlineRadius` / `outlineColor` у класах `Block` та `UnitType`.

### Перевизначення

Можливо перевизначити існуючі спрайти; для цього спрайти повинні бути розміщені в `sprites-override/`.

## **Суфікси**

Гра також може шукати кілька спрайтів для одного блоку.

Для турелей гра може шукати суфікс `<назва>-heat` (`test-turret-heat.png`).

Для блоків і крафтерів/плавилень гра може шукати `<назва>-top` і `<назва>-liquid`, які будуть задокументовані в їхньому розділі.

Для отримання додаткової інформації ви можете переглянути вихідний код для кожного відповідного класу блоків, щоб дізнатися, які спрайти вони можуть завантажувати. Дивіться рядки з `@Load`.
Для спрайтів у модах перевірте кожен метод `load()` в класі блоку, якщо такий є.

## **Колірна палітра**

Як і в кожній грі, в Mindustry є своя колірна палітра. Для початківців наполегливо рекомендується дотримуватися цих конкретних кольорів для ваших спрайтів, інакше вони можуть виглядати недоречно в кращому випадку і навіть стати єретичними в гіршому. Це може викликати велике обурення в Discord-каналі #spriting.

Колірна палітра блоків:

![Палітра Mindustry](/.gitbook/images/modding/spriting/pal-mindustry.png)

Колірна палітра середовища:

![Палітра Mindustry оточення](/.gitbook/images/modding/spriting/pal-mindustry-evn.png)

Припускаючи, що ви правильно придбали відповідне програмне забезпечення для спрайтингу, ви повинні мати можливість завантажити ці зображення та використовувати їх як колірну палітру.

## **Стилі та тіньування**

Mindustry має простий, але обмежений художній стиль. Те, що може працювати для інших ігор, буде виглядати недоречно в Mindustry. Через це були встановлені керівні принципи, щоб допомогти розробникам модів створювати спрайти, які вписуватимуться в гру.

Mindustry - це 2D-гра, тому для додавання глибини, такої як підвищення і заглиблення, нам потрібно використовувати трюк, який називається 'тіньування'. Незважаючи на те, що актив насправді є 2D-зображенням, цей трюк робить його 3D в грі.

Залежно від того, де світить світло, **підвищення** позначаються **світлішим тоном**, **плоскі ділянки** - **середнім тоном**, а **заглиблення** - **темнішим тоном**. Уявлення чогось у 3D-формі, а потім малювання цього в 2D - зазвичай хороший спосіб створення спрайту в Mindustry.

Це лише керівництво, проте якщо ви відхилитеся від нього, не створивши спочатку успішні спрайти Mindustry, ви, швидше за все, створите щось жахливе, і канал #spriting буде незадоволений.

---

### **Тіньування блоків**

![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/production/surge-smelter.png)

Ми використаємо Surge Smelter як приклад.

У блоках джерело світла знаходиться біля **верхнього правого** кута, а тіні - в **нижньому лівому**. Пікселі у верхній правій частині, які близькі до джерела світла, повинні бути світлих кольорів. Так само, пікселі в правій нижній частині повинні бути темними. Найкраще, коли діагональна лінія проходить через середину, розділяючи їх.

Більшість блоків мають 3 типи кольорів:

  - Базовий колір, який має 3 відтінки:

    - ![](https://via.placeholder.com/15/B0BAC0/000000?text=+) `B0BAC0` | Світлий тон
    - ![](https://via.placeholder.com/15/989AA4/000000?text=+) `989AA4` | Середній тон
    - ![](https://via.placeholder.com/15/6E7080/000000?text=+) `6E7080` | Темний тон

  - Колір деталей, який також має 3 відтінки:

    - ![](https://via.placeholder.com/15/feb380/000000?text=+) `FEB380` | Світлий тон
    - ![](https://via.placeholder.com/15/ea8878/000000?text=+) `EA8878` | Середній тон
    - ![](https://via.placeholder.com/15/bc5452/000000?text=+) `BC5452` | Темний тон

  - Нижній колір

    - ![](https://via.placeholder.com/15/4a4b53/000000?text=+) `4a4b53`

**Базовий колір** представляє основний колір блоку. Рекомендується використовувати лише відтінки сірого для крафтерів, як це роблять усі ванільні крафтери.

**Колір деталей** в блоці - це акцентний колір. Він представляє **роль** або **призначення** блоку і спосіб відрізнити їх один від одного. Щоб вибрати, який колір деталей використовувати для ваших блоків, вам слід подумати про призначення вашого блоку. Наприклад:

**Plastanium Compressor**

![Plast-Comp](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/production/plastanium-compressor.png)

Plastanium Compressor має зелену деталь. Ця зелена деталь має той самий колір, що й пластаній. Тому, просто глянувши на нього, можна сказати, що цей блок має зв'язок з пластанієм.

**Нижній колір** представляє внутрішню частину блоку, куди не потрапляє світло, тому він повинен бути дуже темним. Це може представляти дно блоку з димоходом, наприклад, Surge Smelter.

Зверніть увагу, що різні блоки вимагають різної кількості шарів залежно від їхнього типу; наприклад, стіна потребуватиме лише 1 шар, який є самим спрайтом, тоді як блоки на кшталт реконструктора можуть потребувати до 4. Див. [#суфікси](#суфікси).

Приклади модів:

  - Unit Bunker від Flin#8261 з [DiverseTech](https://github.com/FlinTyX/DiverseTech)

    - ![Unit Bunker](/.gitbook/images/modding/spriting/sprite-examples/flintyx-unit-bunker.png)

  - Steam Press від Geschiedenis #4783 з [Unlimited Armament Works](https://github.com/Eschatologue/Unlimited-Armament-Works)

    - ![](https://raw.githubusercontent.com/Eschatologue/Unlimited-Armament-Works/master/assets/sprites/blocks/production/steam-press.png)


---

### **Тіньування турелей**

При тіньуванні турелей джерело світла знаходиться на **правій стороні**, а тіні - на **лівій**.

![ripple](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/ripple.png)

Ми використаємо '**Ripple**' як приклад для цієї частини.

Турелі загалом мають 2-3 типи кольорів, з 2 тонами для кожного:

- Базовий колір

  - ![](https://via.placeholder.com/15/7b7b7b/000000?text=+) `7B7B7B` | Світлий тон
  - ![](https://via.placeholder.com/15/4d4e58/000000?text=+) `4D4E58` | Темний тон

- Колір деталей

  - ![](https://via.placeholder.com/15/feb380/000000?text=+) `FEB380` | Світлий тон
  - ![](https://via.placeholder.com/15/ea8878/000000?text=+) `EA8878` | Темний тон

- [Опціонально] Колір отвору ствола

  - ![](https://via.placeholder.com/15/2c2d38/000000?text=+) `2C2D38`

**Базовий колір** або колір тіла - це основний колір турелі. Це може бути класичний мідно-коричневий, білий, темно-сірий або кастомний колір (з палітри!).

  - Мідно-коричневий
    - ![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/duo.png) ![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/scorch.png) ![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/hail.png)
    - Зазвичай представляє турель низького рівня, такі як **Duo**, **Scorch**, **Hail** тощо.

      - ![](https://via.placeholder.com/15/c9a58f/000000?text=+) `C9A58F`
      - ![](https://via.placeholder.com/15/8f665b/000000?text=+) `8F665B`

  - Білий

    - ![Arc](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/arc.png) ![Lancer](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/lancer.png) ![Parallax](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/defense/parallax.png) ![Segment](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/defense/segment.png)
    - Зазвичай представляє турелі, які використовують енергію замість предметів для стрільби, такі як **Arc**, **Lancer**, **Paralax**, **Segment**.

      - ![](https://via.placeholder.com/15/f4f4f4/000000?text=+) `F4F4F4`
      - ![](https://via.placeholder.com/15/c1c3d4/000000?text=+) `C1C3D4`

  - Темно-сірий

    - ![Swarmer](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/swarmer.png) ![Cyclone](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/cyclone.png) ![Meltdown](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/meltdown.png)
    - У більшості випадків темно-сірий представляє турелі середнього та високого рівня.

      - ![](https://via.placeholder.com/15/7b7b7b/000000?text=+) `7B7B7B`
      - ![](https://via.placeholder.com/15/4d4e58/000000?text=+) `4D4E58`

**Колір деталей** в турелі такий же, як і у звичайного блоку; це акцентний колір і може представляти роль, призначення або архетип турелі. Наприклад, якщо ви намагаєтеся згрупувати свої турелі в різні класи, ви можете відрізнити їх за кольором деталей.

**Отвір ствола** - це опціональний колір для турелей, який представляє отвір ствола вашої турелі; це зазвичай використовується для артилерійських турелей або ракетних установок.

![Swarmer](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/swarmer.png)
![Ripple](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/blocks/turrets/ripple.png)

  - ![](https://via.placeholder.com/15/2c2d38/000000?text=+) `2C2D38`

#### Нетрадиційні методи

  - **Середній тон турелі**

    - Ще відносно новий нетрадиційний метод - додавання середніх тонів до спрайтів турелей, щоб вони виглядали так, ніби мають плоску поверхню, замість того, щоб мати лише світлі та темні тони.

    - Один з прикладів - "Skyhammer" з [Unlimited Armament Works](https://github.com/Eschatologue/Unlimited-Armament-Works)

      - ![Skyhammer](https://github.com/Eschatologue/Unlimited-Armament-Works/blob/master/assets/sprites/blocks/turrets/artillery/skyhammer/skyhammer-preview.png?raw=true)

---

### **Тіньування ресурсів**

Тіньування ресурсів досить просте і може мати джерело світла з **верхніх кутів**, **зверху донизу** або **справа наліво**.

Спрайти ресурсів повинні використовувати лише 2 або 3 відтінки одного кольору. Переконайтеся, що спрайт виглядає 3D, а не плоским, оскільки в такому випадку він виділятиметься як паперовий.

Приклади:

![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/item-copper.png)
![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/item-plastanium.png)
![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/item-graphite.png)
![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/item-coal.png)
![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/item-surge-alloy.png)
![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/item-scrap.png)
![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/item-pyratite.png)
![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/items/liquid-cryofluid.png)

### **Тіньування юнітів**

Юніти зазвичай найскладніше тіньувати.

Тіньування юнітів може стати досить складним для більших юнітів. У тіньуванні юнітів світло йде **зверху вниз** або **спереду назад**. Інтенсивність світлішого тону та темнішого тону змінюється залежно від того, з якою частиною юніта ви працюєте.

Для юнітів світлий тон представляє **підвищення**, середній тон представляє **плоскі ділянки**, а темний тон представляє **заглиблення**.

#### **Базовий колір юніта**

![Тіньування юніта](/.gitbook/images/modding/spriting/spriting-unit-shading.png)

Eclipse використовується для цього прикладу, оскільки це найскладніший ванільний юніт. Коли ви рухаєтеся до задньої частини, буде менше світлого тону і більше середнього та темного тону.

Частини, освітлені світлом, матимуть світліший тон, в той час як ті, які не освітлені, отримують темніший тон; плоскі ділянки мають середній тон.

![Ілюстрація тіньування юніта](/.gitbook/images/modding/spriting/spriting-unit-shading-illustration.png)

Вище наведені приблизні ілюстрації юнітів, якщо уявити їх у 3D.

- Базовий колір, як завжди, має 3 тони:

  - ![](https://via.placeholder.com/15/B0BAC0/000000?text=+) `B0BAC0` | Світлий тон
  - ![](https://via.placeholder.com/15/989AA4/000000?text=+) `989AA4` | Середній тон
  - ![](https://via.placeholder.com/15/6E7080/000000?text=+) `6E7080` | Темний тон

#### **Колір деталей юніта**

Колір деталей юніта має лише 2 тони: світлий і темний. Колір представляє роль юніта в грі.

- Жовтий колір представляє **Основні** юніти, які виробляє Ядро.

  - ![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/units/gamma.png) ![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/units/beta.png)

    - ![](https://via.placeholder.com/15/ffd37f/000000?text=+) `FFD37F` | Світлий тон
    - ![](https://via.placeholder.com/15/d4816b/000000?text=+) `D4816B` | Темний тон

- Помаранчевий колір представляє **Штурмові** юніти, які мають роль атаки ваших опонентів.

  - ![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/units/fortress.png) ![](https://raw.githubusercontent.com/Anuken/Mindustry/master/core/assets-raw/sprites/units/horizon.png)

