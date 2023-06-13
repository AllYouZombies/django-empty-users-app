# Django Empty Users App

This app can be helpful for migrating to custom user model in existing Django project that already has users in database.

To learn more, please read this:
https://testdriven.io/blog/django-custom-user-model-migration/

I've made an app with 1 empty migration file, so you don't have to create it yourself.

> If you find this packaga useful, please consider giving it a star on [GitHub](https://github.com/AllYouZombies/django-empty-users-app).

## Installation

```shell
pip install django-empty-users-app
```

## Usage

Add `users` to `INSTALLED_APPS` in your `settings.py` file.

```python
INSTALLED_APPS = [
    ...
    'users',
    ...
]
```

Then run migrations:

```shell
python manage.py migrate
```

After performing migrations in all your environments, you can remove this app from `INSTALLED_APPS` and delete it from your project.

## License

[MIT](https://choosealicense.com/licenses/mit/)
