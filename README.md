# Viral Posts Engine

Скилл для Codex / Cursor / Claude: вирусные текстовые посты для Telegram (анонс эфира, саммари, обычный пост).

Ниша — **обязательный параметр**: спрашивает нишу и аудиторию, не фиксируется на одной тематике.

Парный скилл для видео: [viral-reels-engine](https://github.com/kirskryl/viral-reels-engine). Раздавайте вместе.

## Триггеры

`/viral-posts`, `/viral-posts-engine`.

Только по явной команде (`disable-model-invocation: true`). Не автотриггерится на «напиши пост».

## Установка

### Codex

```bash
git clone https://github.com/kirskryl/viral-posts-engine.git ~/.codex/skills/viral-posts-engine
# рекомендуется вместе:
git clone https://github.com/kirskryl/viral-reels-engine.git ~/.codex/skills/viral-reels-engine
```

В `~/.codex/config.toml`:

```toml
[features]
skills = true
```

### Cursor / Claude

```bash
git clone https://github.com/kirskryl/viral-posts-engine.git ~/.cursor/skills/viral-posts-engine
ln -sfn ~/.cursor/skills/viral-posts-engine ~/.claude/skills/viral-posts-engine
```

## Обновление

```bash
git -C ~/.codex/skills/viral-posts-engine pull
# или
git -C ~/.cursor/skills/viral-posts-engine pull
```

## Лицензия

MIT — см. [LICENSE](LICENSE).
