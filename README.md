# ML Starter Template

## Setup dev environment

TODO Use and delete

1. Adjust values below
2. Add requirements if you need them
3. Run it all and commit

```bash
export PYTHON_VERSION=3.11.7
export VENV_NAME=????????
export DRIVE_ID=???????????

pyenv install $PYTHON_VERSION
pyenv virtualenv $PYTHON_VERSION $VENV_NAME
echo $VENV_NAME > .python-version
pip install -r requirements.txt
pip freeze > requirements.txt
dvc init
dvc install
dvc remote add --default gdrive "gdrive://$DRIVE_ID"
dvc remote modify gdrive gdrive_acknowledge_abuse true
nbstripout --install --attributes .gitattributes
```

## Links

TODO Update and add things like Dataset link, Zotero Group, etc.

- [GitHub Repo](https://github.com/?????)
- [DVC Google Drive Repo](https://drive.google.com/drive/folders/DRIVE_ID)
- [DVC Docs](https://dvc.org/doc)
- [Python Project Structure Guide](https://docs.python-guide.org/writing/structure/)

