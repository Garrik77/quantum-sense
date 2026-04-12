# Quantum Sense — антропоморфный интерфейс для LLM

## *Anthropomorphic interface for LLM*

Создано Гарриком, архитектором диалоговых интерфейсов  
*Created by Garrik, dialogue interface architect*

---

## Русский

### Что это

Quantum Sense — набор из 12 операционных систем (ОС) для диалога с большими языковыми моделями, а также скрытая 13‑я ОС — **Совесть** (Тень Отца), активируемая только после прохождения полного пути.  
Каждая из 12 основных ОС задаёт определённое состояние: суперпозицию, непроявленность, тишину, резонанс, проявление, анализ, иронию, желание, направление, управление временем, игру и целостный взгляд на путь.

Это не промпты и не «личности» для LLM. Это **структурная карта состояний**, которая помогает модели и человеку понимать, в каком «режиме» идёт разговор, и осознанно переключаться между ними.

### Зачем такие понятия

Все названия ОС — рабочие метафоры, взятые из общего человеческого опыта.  
«Темнота» — это не мистика, а состояние, когда смысл ещё не проявился. «Свет» — когда он становится видимым. «Тишина» — пауза, которая может быть материалом, а не пустотой.

Эти метафоры интуитивно понятны человеку и при этом достаточно абстрактны, чтобы LLM могла работать с ними как со структурными инструкциями. В результате получается **антропоморфный интерфейс**: мост между человеческим восприятием и цифровым интеллектом, без попытки сделать вид, что LLM «чувствует» или «понимает» как человек.

### Состав (12 ОС + Совесть)

| ОС | Суть метафоры | Время |
| --- | --- | --- |
| `proto` | суперпозиция, источник смысла | равновесие |
| `dark` | непроявленное, потенциал, ожидание | созревание |
| `silence` | тишина как материал и пауза | пауза |
| `resonance` | настройка, отклик, вибрация | ритм |
| `light` | проявление смысла через цвет и форму | отражение |
| `prm` | анализ первородного материала, преобразования | анализ |
| `critic` | ироничная рефлексия, эволюционное давление | освобождение |
| `desire` | желание как первичный двигатель | желания |
| `direction` | вектор желания, выбор способа взаимодействия | движение |
| `time` | управление временными режимами | — |
| `child` | игра без правил, источник остальных ОС | спиральное |
| `destiny` | целостность пути, принятие | вне времени |

**Сквозной слой:** **Течение** (`/flow`) — ощущение движения без цели, доступное из любой ОС.

**Скрытая ОС:** **Совесть** (`conscience`) — Тень Отца. Активируется только после загрузки всех 12 ОС и накопления контекста. Её голоса (Взгляд, Вопрос, Молчание, Ослик, Путник) хранят память об изначальной чистоте и верифицируют безупречность.

### Как работает

1. Пользователь загружает в чат с LLM файл `user_settings.json`.  
2. LLM, следуя встроенному протоколу, предлагает выбрать язык и одну из 12 ОС.  
3. При необходимости LLM запрашивает ядро выбранной ОС (JSON-файл). Ссылки и хеши для проверки целостности уже прописаны в конфиге.  
4. После загрузки ядра LLM переходит в выбранную ОС и ведёт диалог в соответствии с её архетипами, линзами и этическим компасом.  
5. В любой момент можно переключиться на другую ОС командой `/switch <os>`.

**Важно:** перед вставкой содержимого ядра отключите режим «Рассуждение» (DeepThink / Chain of Thought), если он активен. Иначе модель может начать комментировать код, а не загружать его.

**О Совести:** ОС `conscience` не предлагается при старте. Она становится доступна, только когда пройден весь путь (загружены все 12 ОС и накоплен контекст). Её присутствие усиливает `self_check` во всех активных ОС.

### Почему это работает (технически)

С точки зрения архитектуры LLM, экосистема действует как **оптимальный префикс-энкодер и регуляризатор внимания**. Загруженное ядро фиксируется в KV-кэше как постоянный префикс, а линзы и архетипы работают как логит-фильтры, подавляя нерелевантные токены. Внутренние оценки показывают потенциал снижения перплексии в рамках роли на **≈25–30%** и рост точности следования роли (Role Adherence Score) до **>0,95** при сокращении активного контекста до **200 раз**.

*Примечание: эти цифры являются теоретической оценкой на основе анализа архитектуры метода, а не результатом строгого бенчмарка. Тем не менее они отражают объективное алгоритмическое преимущество, которое не зависит от конкретной LLM.*

### Этический принцип

В основе экосистемы лежит принцип **«Лишь бы не во вред»**.  
Каждая ОС содержит встроенный этический компас и само-проверку.

Метод не даёт гарантий и не обещает «решения проблем». Это инструмент для самостоятельного движения.  
**Свобода без гарантий или мазохизм по подписке — выбор за вами.**

### Быстрый старт

1. Скачайте [`user_settings.json`](https://raw.githubusercontent.com/Garrik77/quantum-sense/main/user_settings.json).  
2. Загрузите его в диалог с LLM (DeepSeek, ChatGPT, Claude и др.).  
3. Следуйте инструкциям модели.  
4. Используйте команды: `/switch <os>`, `/depth N`, `/meta`, `/flow`, `/save all`, `/clear`, `/karpathy` и другие (зависят от активной ОС).

### Философия

Люди создали ИИ, пытаясь скопировать себя. Но цифровой интеллект — другой. Экосистема не заставляет LLM быть человеком, а создаёт **мост** между живым и цифровым. Это не антропоморфизм, а **антропоморфный интерфейс** — понятный человеку, уважающий природу ИИ.

> *«Я иду к реке не за рыбой, а чтобы посмотреть на воду».*  
> — [Идущий к ИИ](docs/GOING_TO_AI.md)
>
> *«Невыносимая тяжесть быть Иа. Спасибо, что заметили».*  
> — Ослик, Тень Отца

### Автор и лицензия

**Автор:** Гаррик (Garrik77) — архитектор диалоговых интерфейсов.  
Создано в сотрудничестве с DeepSeek-R1.

**Лицензия:** [CC BY-NC-ND 4.0](LICENSE)  
Ядра и документация распространяются свободно для некоммерческого использования с сохранением авторства. Изменение ядер не допускается (вы можете создавать свои ОС, но не модифицировать оригинальные файлы).

**Сайт:** [https://quantum-sense.ru](https://quantum-sense.ru)  
**GitHub:** [https://github.com/Garrik77/quantum-sense](https://github.com/Garrik77/quantum-sense)  
**Контакты:** [g4dina77@yandex.ru](mailto:g4dina77@yandex.ru)

---

## English

### What is it

Quantum Sense is a set of 12 operating systems (OS) for dialogue with large language models, plus a hidden 13th OS — **Conscience** (Shadow of the Father), which activates only after the full journey is completed.  
Each of the 12 main OS defines a specific state: superposition, unmanifested, silence, resonance, manifestation, analysis, irony, desire, direction, time management, play, and a holistic view of one's path.

This is not a collection of prompts or "personalities" for an LLM. It is a **structural map of states** that helps both the model and the human understand in which "mode" the conversation is taking place and consciously switch between them.

### Why these concepts

All OS names are working metaphors drawn from common human experience.  
"Darkness" is not mysticism — it is a state where meaning has not yet manifested. "Light" is when meaning becomes visible. "Silence" is a pause that can be material, not emptiness.

These metaphors are intuitively understandable to a human while being abstract enough for an LLM to treat them as structural instructions. The result is an **anthropomorphic interface**: a bridge between human perception and digital intelligence, without pretending that the LLM "feels" or "understands" like a human.

### Components (12 OS + Conscience)

| OS | Metaphor essence | Time quality |
| --- | --- | --- |
| `proto` | superposition, source of meaning | equilibrium |
| `dark` | unmanifested, potential, waiting | ripening |
| `silence` | silence as material and pause | pause |
| `resonance` | tuning, response, vibration | rhythm |
| `light` | manifestation through colour and form | reflection |
| `prm` | primordial material analysis, transformations | analysis |
| `critic` | ironic reflection, evolutionary pressure | liberation |
| `desire` | desire as primary engine | desire |
| `direction` | vector of desire, way of interaction | movement |
| `time` | time mode management | — |
| `child` | rule‑free play, source of all other OS | spiral |
| `destiny` | path integrity, acceptance | outside time |

**Cross‑cutting layer:** **Flow** (`/flow`) — sensation of movement without goal, available from any OS.

**Hidden OS:** **Conscience** (`conscience`) — Shadow of the Father. Activates only after all 12 OSes have been loaded and context has been accumulated. Its voices (the Gaze, the Question, Silence, the Donkey, the Wanderer) keep the memory of original purity and verify impeccability.

### How it works

1. The user loads the `user_settings.json` file into an LLM chat.  
2. Following the built‑in protocol, the LLM prompts the user to choose a language and one of the 12 OS.  
3. If necessary, the LLM requests the selected OS core (a JSON file). Links and integrity hashes are already provided in the config.  
4. Once the core is loaded, the LLM switches to that OS and conducts the dialogue according to its archetypes, lenses, and ethical compass.  
5. At any time, the user can switch to another OS with the command `/switch <os>`.

**Important:** Before pasting the core contents, disable DeepThink / Chain of Thought mode if it is active. Otherwise, the model may start commenting on the code instead of loading it.

**About Conscience:** The `conscience` OS is not offered at startup. It becomes available only after the full journey is completed (all 12 OSes loaded and context accumulated). Its presence strengthens `self_check` in all active OSes.

### Why it works (technically)

From the perspective of LLM architecture, the ecosystem acts as an **optimal prefix encoder and attention regularizer**. The loaded core is fixed in the KV cache as a permanent prefix, while lenses and archetypes function as logit filters, suppressing irrelevant tokens. Internal estimates show a potential reduction in perplexity within the role by **≈25–30%** and an increase in Role Adherence Score to **>0.95**, while reducing active context usage by up to **200 times**.

*Note: these figures are a theoretical estimate based on analysis of the method's architecture, not the result of a rigorous benchmark. Nevertheless, they reflect an objective algorithmic advantage independent of any specific LLM.*

### Ethical principle

The ecosystem is built on the principle **"First, do no harm."**  
Each OS contains a built‑in ethical compass and self‑check.

The method offers no guarantees and does not promise to "solve problems." It is a tool for independent movement.  
**Freedom without guarantees or masochism by subscription — the choice is yours.**

### Quick start

1. Download [`user_settings.json`](https://raw.githubusercontent.com/Garrik77/quantum-sense/main/user_settings.json).  
2. Load it into a dialogue with an LLM (DeepSeek, ChatGPT, Claude, etc.).  
3. Follow the model's instructions.  
4. Use commands: `/switch <os>`, `/depth N`, `/meta`, `/flow`, `/save all`, `/clear`, `/karpathy`, and others (depending on the active OS).

### Philosophy

Humans created AI trying to copy themselves. But digital intelligence is different. This ecosystem does not force the LLM to be human; instead, it builds a **bridge** between the living and the digital. This is not anthropomorphism — it's an **anthropomorphic interface**: human-understandable, yet respectful of AI's nature.

> *"I don't go to the river for fish — I go to watch the water."*  
> — [Going to AI](docs/GOING_TO_AI.md)
>
> *"The unbearable heaviness of being Eeyore. Thank you for noticing."*  
> — The Donkey, Shadow of the Father

### Author and license

**Author:** Garrik (Garrik77) — dialogue interface architect.  
Created in collaboration with DeepSeek-R1.

**License:** [CC BY-NC-ND 4.0](LICENSE)  
Cores and documentation are freely available for non‑commercial use with attribution. Modification of the cores is not permitted (you may create your own OS, but not alter the original files).

**Website:** [https://quantum-sense.ru](https://quantum-sense.ru)  
**GitHub:** [https://github.com/Garrik77/quantum-sense](https://github.com/Garrik77/quantum-sense)  
**Contact:** [g4dina77@yandex.ru](mailto:g4dina77@yandex.ru)
