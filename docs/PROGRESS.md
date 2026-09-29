# Журнал проекта

## Текущий статус
Лаба: L1. Часть A (среда) и часть B (упражнения E1–E6) готовы, PR lab/L1-dart-exercises
на ревью. Осталась часть C (мини-спецификация) и PDF-отчёт.

## Сделано
- 2026-09-22: Flutter 3.47.5, Android SDK 36 (без Android Studio), эмулятор Pixel API 35.
- 2026-09-22: hello_pam запущен на emulator-5554, счётчик и hot reload работают.
- 2026-09-22: репозиторий, ruleset protect-main (только через PR).
- 2026-09-29: общий контекст проекта: CODING_STANDARDS.md, TASK.md, PROGRESS.md.
- 2026-09-29: E1–E6 в dart_exercises/ (по файлу и коммиту на упражнение), вывод всех
  примеров совпадает с ТЗ; ограничения проверены: в E1 нет `!`, в E2 нет for/while,
  в E4 Set из двух равных студентов даёт 1, в E6 задержка ~2 с и верный порядок строк.
- 2026-09-29: docs/EXPLAIN/L1.md — разбор каждого упражнения и ответы на контрольные
  вопросы из ТЗ (??/?./!, final/const, async/await против блокировки и then).

## Принятые решения
- Эмулятор: API 35 arm64-v8a (образа для 36 не было).
- Xcode и Chrome не ставим: по ТЗ iOS необязателен, веб не нужен.
- Правила проекта — docs/CODING_STANDARDS.md; CLAUDE.md и AGENTS.md — ссылки на него.
- dart_exercises/ — отдельный Dart-пакет с минимальным pubspec.yaml (без зависимостей);
  проверка — `dart analyze` и `dart format --set-exit-if-changed` вместо
  `flutter analyze`/`flutter test`, т. к. это не Flutter-проект.
- dart в PATH — Homebrew Dart 3.13.4 (не встроенный во Flutter); подходит под ТЗ (3.9+).

## Следующий шаг
Смёржить PR lab/L1-dart-exercises, затем часть C: мини-спецификация T2 FitTrack на 1 страницу
(экраны, сущности Exercise/WorkoutSession, мотивация) и сборка отчёта PAM_L1_*.pdf.
