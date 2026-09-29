# Журнал проекта

## Текущий статус
Лаба: L1. Среда готова, следующий шаг — упражнения E1–E6.

## Сделано
- 2026-09-22: Flutter 3.47.5, Android SDK 36 (без Android Studio), эмулятор Pixel API 35.
- 2026-09-22: hello_pam запущен на emulator-5554, счётчик и hot reload работают.
- 2026-09-22: репозиторий, ruleset protect-main (только через PR).
- 2026-09-29: общий контекст проекта: CODING_STANDARDS.md, TASK.md, PROGRESS.md.

## Принятые решения
- Эмулятор: API 35 arm64-v8a (образа для 36 не было).
- Xcode и Chrome не ставим: по ТЗ iOS необязателен, веб не нужен.
- Правила проекта — docs/CODING_STANDARDS.md; CLAUDE.md и AGENTS.md — ссылки на него.

## Следующий шаг
E1–E6 в dart_exercises/, каждое отдельным коммитом, одним PR lab/L1-dart-exercises.
