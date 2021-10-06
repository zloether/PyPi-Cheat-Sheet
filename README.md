# PyPi Cheat Sheet

## Packaging
1. Create virtual environment
	```
	python3 -m venv env
	```
1. Install build tools
	```
	env/bin/pip3 install build twine
	```
1. Create package
	```
	env/bin/python3 -m build
	```
1. Upload package to PyPi test
	```
	env/bin/python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
	```
1. Install package from PyPi test
	```
	env/bin/pip3 install --index-url https://test.pypi.org/simple/ --no-deps example-pkg-your-username==<version>
	```
1. Upload package to PyPi
	```
	env/bin/python3 -m twine upload dist/*
	```


[https://packaging.python.org/tutorials/packaging-projects/](https://packaging.python.org/tutorials/packaging-projects/)