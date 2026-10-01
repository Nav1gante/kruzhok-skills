# Скиллы кружка вайбкодеров

Скиллы для встреч кружка. Работают в Claude Code (приложение Claude, вкладка Code) и в Codex (приложение ChatGPT, режим Codex).

| Скилл | Встреча | Что делает |
|---|---|---|
| `anketa` | №1 | Собирает HTML-страницу «Анкета обо мне» в стиле школьной анкеты: вопросы раундами → бриф → сборка → правки |

## Установка

### Claude Code (приложение Claude, вкладка Code)

Откройте любую папку и напишите в чат:

> Установи скилл: скачай папку `skills/anketa` из репозитория https://github.com/Nav1gante/kruzhok-skills и положи её в папку `.claude/skills/anketa` в моей домашней папке. Потом проверь, что внутри есть SKILL.md.

Claude попросит разрешение на действия — разрешите. После установки начните новую сессию и напишите `/anketa`.

Если пользуетесь терминалом: `/plugin marketplace add Nav1gante/kruzhok-skills`, затем `/plugin install kruzhok@kruzhok`.

### Codex (приложение ChatGPT, режим Codex)

Напишите в чат:

```
$skill-installer install https://github.com/Nav1gante/kruzhok-skills/tree/main/skills/anketa
```

Разрешите доступ к сети, когда приложение спросит. После установки перезапустите приложение и напишите `$anketa` (или просто «давай делать анкету»).

## Рядом пригодится: frontend-design

Скилл от Anthropic, который делает страницы менее шаблонными. Скилл анкеты использует его, если он установлен.

- **Claude:** кнопка **+** рядом с полем ввода → **Plugins** → **Add plugin** → найти `frontend-design` → установить.
- **Codex:** в чат
  ```
  $skill-installer install https://github.com/anthropics/skills/tree/main/skills/frontend-design
  ```
