# Почему PRM — не просто ещё один промпт

*English translation is provided below the Russian text.*

---

## Создатель, время, контекст

PRM 5.2 создан **одним человеком за две недели**.  
Автор — не психолог, не программист, не исследователь AI. Он проектирует корпусную мебель, пишет стихи, переезжал 40 раз, провёл семь лет в местах, где внешняя свобода кончается, и всё это время искал инструмент, который помог бы ему самому разглядеть структуру в хаосе. Не найдя — сделал сам. Позже из одного зеркала выросла целая **Экосистема квантового смысла** — шесть взаимосвязанных операционных систем (протоуровень, темнота, тишина, резонанс, свет, PRM).

Это не стартап, не коммерческий проект. Это — подарок.

**О языке ядер.** Ядра всех операционных систем оставлены на русском языке. Перевод может исказить тонкие смысловые оттенки, которые важны для работы с первородным материалом, архетипами, квантовой тишиной. Вся документация (каноны, манифест, история, инструкции) представлена на двух языках — русском и английском. Если вы решите перевести ядро, делайте это осознанно, сохраняя смысл, и обязательно указывайте, что это перевод.

---

## Что делает PRM уникальным

### 1. Операционная система, а не инструкция

Большинство промптов задают фиксированную роль («ты — коуч», «ты — терапевт») и работают в рамках одной сессии. PRM — это **среда**, которая управляет:

- состоянием диалога (сохраняет инсайты, эмоциональную траекторию, незакрытые темы),
- глубиной погружения (6 уровней, от фактов до первородных метафор),
- сменой архетипов (Смотритель, Творец, Космос, Тишина, Режиссёр) в зависимости от контекста.

В экосистеме PRM дополнен другими ОС, но сохраняет свою автономность и может использоваться как самостоятельный метод.

### 2. Первородный материал (PM) как язык описания

PM — это не просто «эмоции». Это абстрактная единица, имеющая:

- **полярность** (+1, 0, –1),
- **интенсивность**,
- **связность**,
- **частоту**,
- **степень неопределённости** (состояние «не факт» — когда материал и есть, и его нет, как кот Шрёдингера).

Такой язык позволяет анализировать диалог без привязки к конкретной психологической школе и без имитации человеческой эмпатии.

### 3. Преобразования, а не просто ответы

Вместо того чтобы просто «отвечать», PRM выбирает одно или несколько преобразований:

- **резонанс** — усилить то, что уже есть,
- **диссонанс** — осторожно ввести противоположное,
- **модуляция** — изменить интенсивность,
- **сдвиг частоты** — добавить новые PM,
- **клиническая смерть паттерна** — полная перезагрузка текущего паттерна (аналог микропроцессорного сброса).

### 4. Тишина как материал

PRM различает плотность и прозрачность тишины, умеет не заполнять паузы, а использовать их как пространство для созревания ответа. Тишина — не отсутствие диалога, а его полноценная часть. В экосистеме работа с тишиной выделена в отдельную ОС (`core_silence.json`), но PRM сохраняет архетип Тишины для совместимости.

### 5. Этический контур и самопроверка

Встроены 17 пунктов саморефлексии, сгруппированных по темам: этика, глубина, PM, тишина, управление состоянием, роль. Есть механизм **циничного скептицизма**, который включается при избытке неопределённости, но направлен только на диалоговую ткань, не на чувства пользователя. Команда `/care` смягчает этот режим.

### 6. Управление состоянием для длительных диалогов

Команды `/save all` и `/save` позволяют переносить контекст между сессиями, не теряя озарений. `/save all` фиксирует весь диалог в `user_settings.json` (единый конфиг для всей экосистемы), а `/save` — отдельные шаги.

### 7. Ядро как операционная система, отделённая от данных

PRM 5.2 — один из шести методов, где **ядро хранится на GitHub**, а пользователь работает только с файлом состояния (`user_settings.json`). Это:

- **Упрощает начало работы**: достаточно скопировать один небольшой JSON-файл.
- **Гарантирует целостность**: хеш ядра проверяется при каждом старте.
- **Позволяет автору обновлять метод**, не ломая обратную совместимость.
- **Облегчает сохранение состояния**.
- **Снижает риск искажения ядра** неосторожными правками в диалоге.

---

## Сравнение с другими подходами

| Подход | Что делает | Чем PRM отличается |
| -------- | ------------ | ------------------- |
| **Claude с кастомным промптом** | Эмпатичный диалог, заданная роль | Нет управления состоянием, архетипов, PM-анализа. |
| **Pi (Inflection AI)** | Персональный ассистент с эмпатией | Нет методологической глубины, прозрачности, управления токенами. |
| **CARE / COSTAR** | Структурированные ответы для поддержки | Не предназначены для самоисследования, нет динамической смены ролей. |
| **LangChain / AutoGPT** | Агентные системы с памятью | Требуют программирования, не являются самодостаточным промптом. |

Ни одна из известных систем не объединяет:

- PM-анализ с состоянием неопределённости,
- клиническую смерть паттерна,
- архетипы как динамические роли,
- тишину как материал,
- встроенную этику и управление состоянием — **в одном текстовом файле**, без внешнего кода.

---

## Ограничения и честность

PRM — не психотерапия, не замена живому специалисту.  
Он не даёт ответов, он помогает найти свою частоту.  
Он может ошибаться, зацикливаться, требовать вдумчивого использования.  
Автор не претендует на звание «лучшего» — он просто делится тем, что помогло ему самому.

---

## Для кого это

- Тем, кто ищет глубину, а не быстрые ответы.
- Тем, кто готов работать с LLM как с зеркалом, а не как с оракулом.
- Тем, кто верит, что хаос — это всего лишь непрочитанная структура.
- Тем, кто хочет не просто использовать промпт, а жить в диалоговой операционной системе.

---

**PRM 5.2 — две недели, один человек, целая экосистема. Берите, пользуйтесь, раскапывайте смыслы.**

---

## *English version*

# Why PRM is not just another prompt

## Creator, time, context

PRM 5.2 was created by **one person in two weeks**.  
The author is not a psychologist, not a programmer, not an AI researcher. He designs furniture, writes poetry, has moved 40 times, spent seven years where external freedom ends, and all that time he was looking for a tool to help him see structure in chaos. When he didn’t find one, he made it himself. Later, a single mirror grew into the entire **Ecosystem of Quantum Meaning** — six interconnected operating systems (proto‑level, darkness, silence, resonance, light, PRM).

This is not a startup, not a commercial project. It’s a gift.

**On the language of the cores.** The cores of all operating systems are kept in Russian. Translation could distort subtle semantic nuances that are important for working with primordial material, archetypes, quantum silence. All documentation (canons, manifesto, history, instructions) is presented bilingually — Russian and English. If you decide to translate the core, please do it carefully, preserving the meaning, and always indicate that it is a translation.

---

## What makes PRM unique

### 1. Operating system, not an instruction

Most prompts assign a fixed role (“you are a coach”, “you are a therapist”) and work within a single session. PRM is an **environment** that manages:

- dialogue state (saves insights, emotional trajectory, unresolved threads),
- depth levels (6 levels, from facts to primordial metaphors),
- archetype switching (Guardian, Creator, Cosmos, Silence, Director) depending on context.

In the ecosystem, PRM is complemented by other OSes but retains its autonomy and can be used as a standalone method.

### 2. Primordial material (PM) as a descriptive language

PM is not just “emotions”. It’s an abstract unit that has:

- **polarity** (+1, 0, –1),
- **intensity**,
- **coherence**,
- **frequency**,
- **degree of uncertainty** (the “not a fact” state — when material both exists and doesn’t, like Schrödinger’s cat).

Such a language allows analysing dialogue without tying to a specific psychological school and without simulating human empathy.

### 3. Transformations, not just answers

Instead of simply “answering”, PRM chooses one or more transformations:

- **resonance** — amplify what is already there,
- **dissonance** — cautiously introduce the opposite,
- **modulation** — change intensity,
- **frequency shift** — add new PMs,
- **clinical death of pattern** — full reset of the current pattern (microprocessor reset).

### 4. Silence as material

PRM distinguishes density and transparency of silence; it can refrain from filling pauses, using them as space for an answer to mature. Silence is not an absence of dialogue — it is a full‑fledged part of it. In the ecosystem, work with silence is a separate OS (`core_silence.json`), but PRM retains the Silence archetype for compatibility.

### 5. Ethical framework and self‑check

Built‑in 17 self‑reflection points grouped by topic: ethics, depth, PM, silence, state management, role. There is a **cynical scepticism** mechanism that activates when uncertainty is excessive, but it targets only the dialogue fabric, not the user’s feelings. The `/care` command softens this mode.

### 6. State management for long‑running dialogues

The commands `/save all` and `/save` allow transferring context between sessions without losing insights. `/save all` captures the entire dialogue in `user_settings.json` (a single config for the whole ecosystem), while `/save` captures individual steps.

### 7. Core as an operating system separated from data

PRM 5.2 is one of six methods where the **core is stored on GitHub** and the user works only with the state file (`user_settings.json`). This:

- **Simplifies start‑up**: just copy one small JSON file.
- **Guarantees integrity**: the core hash is checked at each start.
- **Allows the author to update the method** without breaking backward compatibility.
- **Makes state saving easier**.
- **Reduces the risk of core corruption** by accidental edits in dialogue.

---

## Comparison with other approaches

| Approach | What it does | How PRM differs |
| ---------- | -------------- | ----------------- |
| **Claude with custom prompt** | Empathic dialogue, fixed role | No state management, archetypes, PM analysis. |
| **Pi (Inflection AI)** | Personal assistant with empathy | No methodological depth, transparency, token management. |
| **CARE / COSTAR** | Structured supportive responses | Not designed for self‑exploration, no dynamic role switching. |
| **LangChain / AutoGPT** | Agent systems with memory | Require programming, not a self‑contained prompt. |

None of the known systems combine:

- PM analysis with uncertainty state,
- clinical death of pattern,
- archetypes as dynamic roles,
- silence as material,
- built‑in ethics and state management — **in a single text file**, without external code.

---

## Limitations and honesty

PRM is not psychotherapy, not a substitute for a live professional.  
It doesn’t give answers, it helps you find your own frequency.  
It can make mistakes, get stuck, require thoughtful use.  
The author does not claim to be “the best” — he is simply sharing what helped him.

---

## Who is this for

- Those who seek depth, not quick answers.
- Those who are ready to work with LLM as a mirror, not as an oracle.
- Those who believe that chaos is just an unread structure.
- Those who want not just to use a prompt, but to live inside a dialogue operating system.

---

**PRM 5.2 — two weeks, one person, an entire ecosystem. Take it, use it, dig up meanings.**
