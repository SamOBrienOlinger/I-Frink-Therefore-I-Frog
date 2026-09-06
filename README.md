# I Frink, Therefore I Frog · Blog

A Django blog project based on the Code Institute CodeStar learning application.

**Python · Django**

[Getting started](#getting-started) · [Repository guide](#repository-guide) · [Checks](#checks-and-review) · [Credits](#credits-and-reuse)

## What you can explore

- Post and comment models.
- Account views and templates using Django Allauth.
- Rich-text editing and Cloudinary media integration.

## Getting started

Requires Git, Python, pip and a virtual environment. Dependency pins in older projects may need a compatible Python environment; this README does not upgrade them.

```bash
git clone https://github.com/SamOBrienOlinger/I-Frink-Therefore-I-Frog.git
cd I-Frink-Therefore-I-Frog
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

On Windows, activate the environment with `.venv\Scripts\Activate.ps1` instead.

After resolving the project notes and configuring the local environment, use:

```bash
python manage.py check
python manage.py migrate
python manage.py runserver
```

Open [localhost:8000](http://localhost:8000). Stop the server with **Ctrl+C**. Use `python manage.py createsuperuser` in the same project directory if you need access to Django admin.

## Configuration

Settings are defined in [codestar2022/settings.py](codestar2022/settings.py). Set the values used by your chosen local configuration before running Django. A `.env` file is only read when the project explicitly loads it; most of these projects read the process environment or an optional `env.py`.

| Variable | Purpose |
| --- | --- |
| `DATABASE_URL` | Connection URL for your own development database. Required where settings parse it without a fallback. |
| `DEVELOPMENT` | Development-mode switch used when choosing local settings. |
| `SECRET_KEY` | Django signing key. Use a locally generated value and keep it out of Git. |

Use a disposable development database for migrations and tests. Keep service credentials and local configuration out of commits.

## Repository guide

| Path | Purpose |
| --- | --- |
| [requirements.txt](requirements.txt) | Python dependency versions |
| [manage.py](manage.py) | Django management commands |
| [codestar2022/settings.py](codestar2022/settings.py) | Django configuration |
| [templates/](templates/) | Server-rendered page templates |

## Checks and review

From the directory containing `manage.py`, run `python manage.py check` and `python manage.py test` after configuring an isolated development database. Inspect the test modules: scaffold `tests.py` files may contain no actual tests.

Generate fresh results from the revision you are working on; historical test reports describe earlier runs.

## Deployment

Hosting entry points are recorded in [Procfile](Procfile). Configure the runtime, database, allowed origins and static/media handling for the chosen host. Historical deployment records may describe services that are no longer available.

## Credits and reuse

Learning resources and starter material: [Code Institute](https://codeinstitute.net/).

No repository-level licence file is present in this snapshot. This README does not grant additional reuse permissions. Check with the relevant rights holders before reusing code, written content or assets.

## Support

Repository maintained in [Sam O’Brien-Olinger’s GitHub account](https://github.com/SamOBrienOlinger). For a problem or suggested improvement, [open an issue](https://github.com/SamOBrienOlinger/I-Frink-Therefore-I-Frog/issues) with the affected page or command, steps to reproduce, and expected behaviour.

[Back to top](#i-frink-therefore-i-frog--blog)
