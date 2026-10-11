# DataConverter

Учебный CLI-проект для конвертации табличных данных между CSV, JSON и YAML.
Лабораторная работа № 6 — CI-конвейер на GitHub Actions.

СИБГУТИ · Егоров Андрей · ИП-311

## Локальная сборка

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build --config Release
ctest --test-dir build -C Release --output-on-failure
```

## CI

Workflow `.github/workflows/ci.yml` запускается на `push` и `pull_request`.
Сборка и тесты выполняются на `ubuntu-latest`, `macos-latest` и `windows-latest`.
