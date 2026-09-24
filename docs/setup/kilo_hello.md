# Kilo hello

готов

1. Учебный сервис предварительной оценки заявки на заём под ПТС: принимает заявку (VIN, год, пробег, оценочная стоимость, сумма, срок), считает LTV и возвращает решение approve / review / reject (README.md).
2. Makefile: `make up`, `make down`, `make ps`, `make logs`, `make install`, `make test`, `make lint`, `make seed`, `make help`; в docker-compose.yml — сервисы backend (порт `${APP_PORT:-8080}`) и db (MySQL 8.0, порт `${DB_PORT:-3307}`), команд запуска/проверки в нём нет.
3. Решение approve / review / reject считается в `backend/src/Domain/` — класс `DecisionEngine` (backend/src/Domain/DecisionEngine.php).

модель: MiniMax M3 (`openrouter/minimax/minimax-m3` — kilo.jsonc)

токены/стоимость (OpenRouter → Activity): заполнить вручную — у агента нет доступа к OpenRouter