# Viral Posts Engine

Скилл для Cursor / Claude: вирусные текстовые посты для Telegram (анонс эфира, саммари после эфира, обычный пост).

Методология адаптирована из разбора вирусных Reels под текст: первая строка, ритм абзацев, конкретика.

## Триггеры

`/viral-posts`, `/viral-posts-engine`.

Только по явной команде (`disable-model-invocation: true`). Не автотриггерится на «напиши пост».

Ниши по умолчанию: отношения, психология, здоровье, эзотерика.

## Установка

```bash
git clone https://github.com/kirskryl/viral-posts-engine.git ~/.cursor/skills/viral-posts-engine

# опционально — зеркало для Claude Code:
ln -sfn ~/.cursor/skills/viral-posts-engine ~/.claude/skills/viral-posts-engine
```

Файлы:
- [`SKILL.md`](SKILL.md) — протокол, 8 типов постов, чеклист
- [`reference/announcements.md`](reference/announcements.md) — анонс эфира
- [`reference/summaries.md`](reference/summaries.md) — саммари после эфира
- [`reference/hooks-bank.md`](reference/hooks-bank.md) — банк хуков

## Обновление

```bash
git -C ~/.cursor/skills/viral-posts-engine pull
```

## Лицензия

MIT — см. [LICENSE](LICENSE).
