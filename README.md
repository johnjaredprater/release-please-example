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

IMPORTANT: Change some GitHub repo settings:

Settings > General > Scroll down to "Pull Requests" > Only allow rebase merging
Settings > Actions > General > Tick "Allow GitHub Actions to create and approve pull requests"

Make an initial version commit:
```
git commit --allow-empty -m "chore: release 0.1.0" -m "Release-As: 0.1.0"
```