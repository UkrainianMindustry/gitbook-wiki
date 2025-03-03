---
icon: js
---

# Javascript (скриптинг)

Mindustry використовує JavaScript для модифікації скриптів. Скрипти використовують розширення `js` і розміщуються в підкаталозі `scripts/`.

Виконання починається з файлу під назвою `main.js`. Будь-які інші файли скриптів можуть бути імпортовані головним файлом за допомогою `require("script_name")`.
Типова структура виглядає так:

*scripts/main.js*:
```js
require("blocks");
require("items");
```

*scripts/blocks.js*:
```js
const myBlock = extend(Conveyor, "terrible-conveyor", {
    // різні перевизначення...
    size: 3,
    health: 200
    //...
});
```

*scripts/items.js*:
```js
const terribleium = Item("terribleium");
terribleium.color = Color.valueOf("ff0000");
//...
```

# Приклади

## Прослуховування подій

<img src="/wiki/images/misc/modding-pathetic.gif">

```js
// прослуховування події, коли юніт знищено
Events.on(UnitDestroyEvent, event => {
    // показати повідомлення на екрані, коли юніт був гравцем
    if(event.unit.isPlayer()){
        Vars.ui.hudfrag.showToast("Pathetic.");
    }
})
```

Найпростіший спосіб знайти події, які можна прослуховувати, це переглянути вихідний файл: [Mindustry/blob/master/core/src/mindustry/game/EventType.java](https://github.com/Anuken/Mindustry/blob/master/core/src/mindustry/game/EventType.java)

## Відображення діалогового вікна

```js
const myDialog = new BaseDialog("Заголовок діалогу");
// Додати кнопку "повернутися"
myDialog.addCloseButton();
// Додати текст до основного вмісту
myDialog.cont.add("До побачення.");
// Показати діалог
myDialog.show();
```

## Відтворення власних звуків

Відтворення власного аудіо є простим, за умови, що ви зберігаєте свій звуковий кліп у форматі `.mp3` або `.ogg` у вашому каталозі `/sounds`.

Для цього прикладу ми зберегли `example.mp3` у `/sounds/example.mp3`.

### Використання бібліотеки для завантаження звуку

*scripts/alib.js*:
```js
exports.loadSound = (() => {
        const cache = {};
        return (path) => {
                const c = cache[path];
                if (c === undefined) {
                        return cache[path] = loadSound(path);
                }
                return c;
        }
})();
```

*scripts/main.js*:
```js
const lib = require("alib");

Events.on(WaveEvent, event => {
        // завантажує example.mp3
        const mySound = lib.loadSound("example");
        // двигун відтворить цей звук у цій локації (X,Y)
        mySound.at(1, 1);
})
```