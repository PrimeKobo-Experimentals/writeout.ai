# In Original Repo's Issue #3

## How to install this? Can you provide a tutorial?

```bash
$ composer install
$ cp .env.example .env
$ vi .env
```

```conf
# Set below
DB_DATABASE=transcribe_ai
DB_USERNAME=
DB_PASSWORD=
# Beofre running php artisan commands,
# Make sure that you've created a database and
# User has right grants.
```

```sql
mysql -u pma -p
CREATE DATABASE transcribe_ai;
```

```bash
$ php artisan key:generate
$ php artisan migrate
$ php artisan serve
```

If it faield, add OPEN AI's API-Key to .env and rerun `php artisan serve”.

Still got error?

Refer [here](https://github.com/beyondcode/writeout.ai/issues/3)
