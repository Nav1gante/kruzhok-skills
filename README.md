# Скиллы кружка вайбкодеров

Работают в Claude Code (приложение Claude, вкладка Code) и в Codex (приложение ChatGPT, режим Codex).

## Что здесь

| Что | Зачем |
|---|---|
| `skills/koval` | Скилл, который прежде чем что-то делать расспрашивает вас раундами вопросов — цель, содержание, вид, поведение, «а что, если…» — и записывает договорённость в `brief.md`. Подходит для любой задачи: страница, гайд, инструмент |
| `prompts/` | Стартовые промпты встреч. Копируете в чат первым сообщением — и скилл знает, что делаем и что спросить |

| Встреча | Промпт |
|---|---|
| №1 — Анкета обо мне | [prompts/anketa.md](prompts/anketa.md) |

## Установка скилла `koval`

### Claude Code (приложение Claude, вкладка Code)

Откройте любую папку и напишите в чат:

> Установи скилл: скачай папку `skills/koval` из репозитория https://github.com/Nav1gante/kruzhok-skills и положи её в папку `.claude/skills/koval` в моей домашней папке. Потом проверь, что внутри есть SKILL.md.

Claude попросит разрешение на действия — разрешите. Начните новую сессию и проверьте: напишите `/` — в списке должен быть `koval`.

Если пользуетесь терминалом: `/plugin marketplace add Nav1gante/kruzhok-skills`, затем `/plugin install kruzhok@kruzhok`.

### Codex (приложение ChatGPT, режим Codex)

Напишите в чат:

```
$skill-installer install https://github.com/Nav1gante/kruzhok-skills/tree/main/skills/koval
```

Разрешите доступ к сети, когда приложение спросит. Перезапустите приложение.

## Второй скилл: frontend-design

Скилл от Anthropic, который делает страницы менее шаблонными.

- **Claude:** кнопка **+** рядом с полем ввода → **Plugins** → **Add plugin** → найти `frontend-design` → установить.
- **Codex:** в чат
  ```
  $skill-installer install https://github.com/anthropics/skills/tree/main/skills/frontend-design
  ```
