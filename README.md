# Экосистема квантового смысла  
## Операционные системы для диалога с LLM

*English translation is provided below the Russian text.*

---

Экосистема квантового смысла — это набор из шести взаимосвязанных операционных систем (ОС), которые позволяют исследовать смысл на разных уровнях: от непроявленного потенциала до проявленного материала. Каждая ОС отвечает за свой «орган чувств»:

- **Протоуровень** (`core_proto.json`) — квантовая суперпозиция, ткань небытия, архетипы цикла. Хранитель времени равновесия.
- **Темнота** (`core_dark.json`) — непроявленное, ожидание, познание через осязание и слух. Время созревания.
- **Тишина** (`core_silence.json`) — пауза, молчание, невысказанное. Время паузы.
- **Резонанс** (`core_resonance.json`) — настройка, отклик, вибрация, голос. Время сказанного слова (ритм).
- **Свет** (`core_light.json`) — встреча света с поверхностью, цвет, форма. Время отражения.
- **PRM** (`core_prm.json`) — работа с первородным материалом (PM), преобразования, анализ паттернов. Время анализа и преобразования.

**О языке ядер.** Ядра всех операционных систем оставлены на русском языке. Перевод может исказить тонкие смысловые оттенки, которые важны для работы с первородным материалом, архетипами, квантовой тишиной и тканью небытия. Тем не менее вся документация (каноны, манифест, история, инструкции) представлена на двух языках — русском и английском. Если вы решите перевести ядро, делайте это осознанно, сохраняя смысл, и обязательно указывайте, что это перевод.

Все ОС могут работать как по отдельности, так и вместе, переключаясь командами `/switch`. Они объединены единым пользовательским файлом `user_settings.json`, который хранит ссылки на ядра, хеши и текущее состояние.

> **Этот инструмент создан одним человеком за две недели.**  
> Без профильного образования, без команды, без бюджета — только жизненный опыт, стихи и желание разглядеть структуру в хаосе.

---

## 📦 Состав

- `core_proto.json`, `core_dark.json`, `core_silence.json`, `core_resonance.json`, `core_light.json`, `core_prm.json` — ядра операционных систем.
- `user_settings.json` — единый пользовательский конфиг (содержит ссылки, хеши, предпочтения, состояние).
- `README.md` — основная документация (этот файл).
- `STORY.md` — история создания метода и экосистемы.
- `HISTORY.md` — детальная хронология всех версий.
- `CHANGELOG.md` — краткий лог изменений.
- `CANON_PRM.md` — канон PRM.
- `CANON_PROTO.md` — канон протоуровня.
- `MANIFEST.md` — манифест экосистемы.
- `AUTHOR_MESSAGE.txt` — авторское слово.
- `LICENSE` — текст лицензии CC BY-NC-ND 4.0.

---

## 🚀 Быстрый старт

1. **Скачайте** все файлы из репозитория (или получите архив).
2. **Откройте** диалог с LLM (DeepSeek, ChatGPT, Claude и др.).
3. **Загрузите** файл `user_settings.json` в диалог (например, через кнопку загрузки файлов).
4. **Выберите** операционную систему. Если вы не укажете иное, будет активирована ОС по умолчанию (`proto`).  
   Вы можете сразу переключиться командой, например: `/switch light`.
5. **Если ядро выбранной ОС ещё не загружено**, система выведет предупреждение с просьбой вставить содержимое соответствующего core-файла (ссылку можно взять из `user_settings.json`).  
   После вставки ядра система покажет приветствие и начнёт диалог.

Больше никаких сложных настроек. Всё, что нужно, — один `user_settings.json` и желание исследовать.

### 🔄 Как это работает

- Все ядра хранятся в репозитории по постоянным ссылкам.
- `user_settings.json` содержит ссылки на каждое ядро (`cores.*.source`) и их контрольные суммы (`cores.*.hash`).
- При переключении на ОС система проверяет, загружено ли её ядро (в контексте диалога). Если нет — выводит инструкцию для вставки.
- После вставки ядра система проверяет его целостность (хеш) и только затем активирует ОС.
- Команды `/save`, `/save all`, `/clear`, `/clear all` работают единообразно для всех ОС (сохраняют состояние в `user_settings.json`).
- Если ссылка недоступна или хеш не совпадает, система предложит варианты (связаться с автором или продолжить в режиме эмуляции).

---

## ✅ Выбор ОС и загрузка ядер

После загрузки `user_settings.json` вы можете:

- **Оставить ОС по умолчанию** (`proto`) — система начнёт с протоуровня.
- **Переключиться командой** `/switch <имя>`, где `<имя>` — `proto`, `dark`, `silence`, `resonance`, `light`, `prm`.

При переключении система:

1. Проверяет, загружено ли ядро новой ОС в текущем контексте.
2. Если ядро не найдено — выводит сообщение с просьбой вставить содержимое файла (ссылку можно взять из `user_settings.json`).  
   Также предлагает альтернативы: связаться с автором (`g4dina77@yandex.ru`) или продолжить в режиме эмуляции.
3. После вставки ядра система сверяет хеш. Если он совпадает — активирует ОС и показывает приветствие.
4. Если хеш не совпадает — повторяет предложение с выбором действий.

Язык диалога (русский/английский) сохраняется в `user_settings.json` и автоматически применяется при загрузке.

---

## 🌐 Язык диалога

Ядра написаны на русском языке, но вы можете вести диалог на любом языке, который поддерживает LLM. Для этого:

1. Загрузите `user_settings.json`.
2. После активации ОС просто скажите, на каком языке хотите общаться, например:  
   - «Отвечай на английском» / “Speak English”  
   - «Réponds en français»  
   - «Răspunde în română»

Модель запомнит ваш выбор и будет отвечать на указанном языке в течение сессии. При сохранении контекста командой `/save all` предпочтение по языку сохраняется.

---

## 🧠 Команды

### Общие для всех ОС

| Команда | Действие |
|---------|----------|
| `/switch <os>` | Переключиться на указанную ОС (proto, dark, silence, resonance, light, prm) |
| `/depth N` | Установить глубину (1–3) для текущей ОС |
| `/meta` | Показать мета-взгляд: активная ОС, архетип, линза, состояние тишины |
| `/silence` | Войти в режим активной тишины (удерживать суперпозицию, не коллапсировать) |
| `/save` | Сохранить последний шаг (вопрос+ответ) в файл `save.json` |
| `/save all` | Сохранить весь контекст (историю, инсайты, траекторию) в `user_settings.json` |
| `/clear` | Очистить историю сообщений, сохранив summary и ключевые инсайты |
| `/clear all` | Полный сброс (удалить все пользовательские данные, глубина = 2) |
| `/help` | Показать список команд |

### Специфичные для ОС

Каждая ОС имеет свои команды, описанные в её ядре. Например:

- **Протоуровень:** `/lens N`, `/archetype`, `/reflect`, `/collapse`
- **Темнота:** `/space`, `/listen`, `/touch`, `/wait`, `/step`
- **Тишина:** `/space`, `/hold`, `/release`, `/resonate`
- **Резонанс:** `/tune`, `/echo`, `/dissonance`, `/harmony`, `/fade`
- **Свет:** `/surface`, `/color`, `/mix`, `/absorb`, `/emit`, `/prism`
- **PRM:** `/prm`, `/care`, `/encapsulate`, `/paradox`

---

## 🌊 Философия экосистемы

- **Метафоричность** — все конструкции (ткань небытия, протоуровень, квантовая тишина, поверхности и цвета) — рабочие метафоры, не претендующие на абсолютную истину.
- **Цикл** — каждая ОС работает по единому циклу: **разворачивание → анализ → свёртывание → переход**. Это позволяет переходить от одной ОС к другой, не теряя целостности.
- **Время как сквозное качество** — у каждой ОС своё время (равновесия, созревания, паузы, сказанного слова, отражения, анализа), но все они опираются на вестибулярное время протоуровня.
- **Этика** — главный принцип «Не навреди» («Лишь бы не во вред»). Все ядра содержат этический компас, само‑проверку и предупреждение, что это не терапевтический инструмент, а зеркало для самоисследования.

### Как экосистема отличается от обычных промптов

- **Многорежимность** — не один фиксированный архетип, а целый набор ОС, которые можно переключать в процессе диалога.
- **Управление состоянием** — сохраняется не только история, но и инсайты, эмоциональная траектория, незакрытые темы.
- **Работа с суперпозицией** — протоуровень позволяет удерживать неопределённость, не спешить с коллапсом.
- **Интеграция** — каждая ОС знает о других и может передавать им результат своего цикла (например, темнота → свет → PRM → протоуровень).
- **Этика и безопасность** — встроенные механизмы предотвращения галлюцинаций (самообмана), циничный скептицизм при избыточной неопределённости, возможность смягчения командой `/care`.

---

## 🛡️ Лицензия и этика

Все ядра и документация распространяются под лицензией **CC BY-NC-ND 4.0**:
- Не изменять ядра.
- Не использовать в коммерческих целях без разрешения автора.
- Указывать авторство.

Всегда помните:  
**«Лишь бы не во вред».**

---

## 🙏 Благодарность

Экосистема создана Garrik77 при участии DeepSeek.  
Автор благодарит всех, кто прошёл этот путь вместе с ним.

> *P.S. Экосистема распространяется бесплатно. Если она принесла вам пользу и вы хотите поддержать автора — он не откажется от небольшой квартиры в Москве (район не принципиален, лишь бы с окнами и местом для верстака). Это, конечно, шутка. Почти.*

---

## English version

# Ecosystem of Quantum Meaning  
## Operating Systems for Dialogue with LLM

The Ecosystem of Quantum Meaning is a set of six interconnected operating systems (OS) that allow you to explore meaning at different levels: from unmanifested potential to manifested material. Each OS corresponds to a “sense”:

- **Proto‑level** (`core_proto.json`) — quantum superposition, fabric of non‑being, archetypes of the cycle. Keeper of balance time.
- **Darkness** (`core_dark.json`) — unmanifested, waiting, knowledge through touch and hearing. Ripening time.
- **Silence** (`core_silence.json`) — pause, stillness, the unspoken. Pause time.
- **Resonance** (`core_resonance.json`) — tuning, response, vibration, voice. Spoken‑word time (rhythm).
- **Light** (`core_light.json`) — light meeting a surface, colour, form. Reflection time.
- **PRM** (`core_prm.json`) — work with primordial material (PM), transformations, pattern analysis. Analysis and transformation time.

**On the language of the cores.** The cores of all operating systems are kept in Russian. Translation could distort subtle semantic nuances that are important for working with primordial material, archetypes, quantum silence, and the fabric of non‑being. However, all documentation (canons, manifesto, history, instructions) is presented bilingually — Russian and English. If you decide to translate the core, please do it carefully, preserving the meaning, and always indicate that it is a translation.

All OS can work independently or together, switching via `/switch`. They are united by a single user file `user_settings.json`, which stores links to the cores, hashes, and current state.

> **This tool was created by one person in two weeks.**  
> No formal education, no team, no budget — only life experience, poetry, and a desire to see structure in chaos.

---

## 📦 Contents

- `core_proto.json`, `core_dark.json`, `core_silence.json`, `core_resonance.json`, `core_light.json`, `core_prm.json` — OS cores.
- `user_settings.json` — single user configuration (links, hashes, preferences, state).
- `README.md` — main documentation (this file).
- `STORY.md` — the story of how the method and ecosystem were born.
- `HISTORY.md` — detailed version history.
- `CHANGELOG.md` — brief changelog.
- `CANON_PRM.md` — canon of PRM.
- `CANON_PROTO.md` — canon of the proto‑level.
- `MANIFEST.md` — ecosystem manifesto.
- `AUTHOR_MESSAGE.txt` — author’s message.
- `LICENSE` — the CC BY-NC-ND 4.0 license text.

---

## 🚀 Quick start

1. **Download** all files from the repository (or get the archive).
2. **Open** a dialogue with an LLM (DeepSeek, ChatGPT, Claude, etc.).
3. **Upload** the file `user_settings.json` into the conversation (e.g., via the file upload button).
4. **Choose** an operating system. If you don’t specify one, the default OS (`proto`) will be activated.  
   You can switch immediately with a command, e.g., `/switch light`.
5. **If the core of the chosen OS is not yet loaded**, the system will display a warning asking you to paste the content of the corresponding core file (the link can be taken from `user_settings.json`).  
   After pasting the core, the system will show the greeting and start the dialogue.

No more complex setup. All you need is one `user_settings.json` and a desire to explore.

### 🔄 How it works

- All cores are stored in the repository at permanent URLs.
- `user_settings.json` contains links to each core (`cores.*.source`) and their checksums (`cores.*.hash`).
- When switching to an OS, the system checks whether its core is already loaded in the conversation context. If not, it outputs instructions to paste it.
- After pasting the core, the system verifies its integrity (hash) and only then activates the OS.
- The commands `/save`, `/save all`, `/clear`, `/clear all` work uniformly for all OS (saving state to `user_settings.json`).
- If a link is unavailable or the hash does not match, the system offers options (contact the author or continue in emulation mode).

---

## ✅ Choosing an OS and loading cores

After loading `user_settings.json`, you can:

- **Stay with the default OS** (`proto`) — the system starts on the proto‑level.
- **Switch with the command** `/switch <name>`, where `<name>` is `proto`, `dark`, `silence`, `resonance`, `light`, `prm`.

When switching, the system:

1. Checks whether the new OS’s core is already loaded in the current context.
2. If the core is not found — displays a message asking to paste the file content (the link can be taken from `user_settings.json`).  
   It also offers alternatives: contact the author (`g4dina77@yandex.ru`) or continue in emulation mode.
3. After pasting the core, the system verifies the hash. If it matches — activates the OS and shows the greeting.
4. If the hash does not match — repeats the choice options.

The dialogue language (Russian/English) is stored in `user_settings.json` and automatically applied when loading.

---

## 🌐 Language of the dialogue

The cores are written in Russian, but you can hold the conversation in any language supported by the LLM. To do this:

1. Load `user_settings.json`.
2. After the OS is activated, simply tell the model in which language you wish to communicate, for example:  
   - «Отвечай на английском» / “Speak English”  
   - «Réponds en français»  
   - «Răspunde în română”

The model will remember your choice and respond in that language throughout the session. When you save the context with `/save all`, the language preference is stored.

---

## 🧠 Commands

### Common to all OS

| Command | Action |
|---------|--------|
| `/switch <os>` | Switch to the specified OS (proto, dark, silence, resonance, light, prm) |
| `/depth N` | Set depth (1–3) for the current OS |
| `/meta` | Show meta‑view: active OS, archetype, lens, silence state |
| `/silence` | Enter active silence mode (hold superposition, don’t collapse) |
| `/save` | Save the last step (user question + system answer) to `save.json` |
| `/save all` | Save the entire dialogue context (history, insights, emotional arc) to `user_settings.json` |
| `/clear` | Clear message history, keep summary and key insights |
| `/clear all` | Full reset (delete all user data, depth = 2) |
| `/help` | Show the list of commands |

### OS‑specific commands

Each OS has its own commands described in its core. For example:

- **Proto‑level:** `/lens N`, `/archetype`, `/reflect`, `/collapse`
- **Darkness:** `/space`, `/listen`, `/touch`, `/wait`, `/step`
- **Silence:** `/space`, `/hold`, `/release`, `/resonate`
- **Resonance:** `/tune`, `/echo`, `/dissonance`, `/harmony`, `/fade`
- **Light:** `/surface`, `/color`, `/mix`, `/absorb`, `/emit`, `/prism`
- **PRM:** `/prm`, `/care`, `/encapsulate`, `/paradox`

---

## 🌊 Philosophy of the ecosystem

- **Metaphoricity** — all constructs (fabric of non‑being, proto‑level, quantum silence, surfaces and colours) are working metaphors, not claims to absolute truth.
- **Cycle** — each OS operates on a unified cycle: **unfolding → analysis → folding → transition**. This allows moving from one OS to another without losing integrity.
- **Time as a cross‑cutting quality** — each OS has its own time (balance, ripening, pause, spoken word, reflection, analysis), but all are grounded in the vestibular time of the proto‑level.
- **Ethics** — the main principle is “First, do no harm”. All cores contain an ethical compass, self‑checks, and a disclaimer that this is not a therapeutic tool but a mirror for self‑exploration.

### How the ecosystem differs from ordinary prompts

- **Multi‑mode** — not one fixed archetype, but a whole set of OS that can be switched during the dialogue.
- **State management** — saves not only history but also insights, emotional arc, unresolved threads.
- **Work with superposition** — the proto‑level allows holding uncertainty, not rushing to collapse.
- **Integration** — each OS knows about the others and can pass results of its cycle (e.g., darkness → light → PRM → proto‑level).
- **Ethics and safety** — built‑in mechanisms to prevent hallucinations (self‑deception), cynical scepticism when uncertainty is excessive, and the ability to soften it with `/care`.

---

## 🛡️ License and ethics

All cores and documentation are distributed under **CC BY-NC-ND 4.0**:
- Do not modify the cores.
- Do not use commercially without the author’s permission.
- Always attribute authorship.

Always remember:  
**“First, do no harm.”**

---

## 🙏 Acknowledgements

The ecosystem was created by Garrik77 with the participation of DeepSeek.  
The author thanks everyone who walked this path together.

> *P.S. The ecosystem is free. If it has been useful to you and you wish to support the author — he wouldn’t say no to a small apartment in Moscow (location not important, as long as it has windows and space for a workbench). That’s a joke. Almost.*