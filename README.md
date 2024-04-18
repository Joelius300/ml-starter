# ML Starter Template

My personal simple ML Starter Template using [pyenv](https://github.com/pyenv/pyenv), [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv), [DVC](https://github.com/iterative/dvc), and [PyTorch Lightning](https://github.com/Lightning-AI/pytorch-lightning). Feel free to use and expand/fork it.

## Use template

This section explains how to do the required one-time setup for the template.

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

## Init dev environment

This section explains how to set up the development environment on any subsequent computer after the template-setup is done and commited.

```
export PYTHON_VERSION=3.11.7

pyenv install $PYTHON_VERSION
pyenv virtualenv $PYTHON_VERSION $VENV_NAME
pip install -r requirements.txt
dvc install
nbstripout --install --attributes .gitattributes
```

## Links

TODO Update and add things like Dataset link, Zotero Group, etc.

- [GitHub Repo](https://github.com/?????)
- [DVC Google Drive Repo](https://drive.google.com/drive/folders/DRIVE_ID)
- [DVC Docs](https://dvc.org/doc)
- [Python Project Structure Guide](https://docs.python-guide.org/writing/structure/)

