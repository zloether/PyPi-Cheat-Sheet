# PyPi Cheat Sheet

## Packaging
1. Create package
	```
	python setup.py sdist
	```
1. Upload package to PyPi test
	```
	python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
	```
1. Install package from PyPi test
	```
	python -m pip install --index-url https://test.pypi.org/simple/ --no-deps example-pkg-your-username
	```
1. Upload package to PyPi
	```
	python -m twine upload dist/*
	```


[https://packaging.python.org/tutorials/packaging-projects/](https://packaging.python.org/tutorials/packaging-projects/)