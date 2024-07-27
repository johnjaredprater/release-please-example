# release-please-example

Using pyenv
```
pyenv local 3.11.4
python -m venv .env311
source .env311/bin/activate
```

```
pip install pre-commit
pre-commit install --hook-type commit-msg
```

Add a dockerhub access token to the GitHub secrets: `DOCKER_ACCESS_TOKEN`

