# README.md

## Notes

DB access: `psql -U bookings_user -d bookings_db`
Run app: `uv run uvicorn bookings.main:create_app --factory --reload`

`uv run ruff format .`
`uv run ruff check .`
`uv run mypy src`

init
`uv run alembic init -t async migrations`

migrate
`uv run alembic revision --autogenerate -m "create resources"`
`uv run alembic upgrade head`
`uv run alembic current` - check current revision