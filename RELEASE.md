# Release Commands

```
pip install twine
bumpversion patch --allow-dirty
python setup.py sdist
twine upload -u ${{ secrets.PYPI_USERNAME }} -p ${{ secrets.PYPI_PASSWORD }} dist/*
```
