# CropDeal Central Configuration

These property files are intended to be stored in the Git repository used by Spring Cloud Config Server.

## Files

- `application.properties` - common configuration
- `<service-name>.properties` - service-specific configuration

## Environment variables

Set these outside Git before running the services:

- `DB_USERNAME`
- `DB_PASSWORD`
- `JWT_SECRET`
- `INTERNAL_API_KEY`
- `CROPDEAL_ADMIN_EMAIL`
- `CROPDEAL_ADMIN_PASSWORD`
- `EUREKA_URL`
- `RABBITMQ_HOST`
- `RABBITMQ_PORT`
- `RABBITMQ_USERNAME`
- `RABBITMQ_PASSWORD`
- `JPA_DDL_AUTO` (optional)
- `JPA_SHOW_SQL` (optional)
- `REVIEW_DB_URL` (optional)

Do not commit real passwords, JWT secrets, API keys, or admin credentials to this repository.

The existing `localhost`, `root`, and `guest` values are only non-secret local-development defaults where present. The database password and admin password are intentionally environment-only.
