# Setting version
Set version: `version.txt`

Typical build will include a `dev` postfix in a version number
Release version requires setting env variable `RELEASE=1` for the build

# Build
Windows:
```shell
# py -m pip install --upgrade build
py -m build
 ```
MacOS:
```shell
# pip install --upgrade build
python -m build
 ```

# Install
Windows:
```shell
 py -m pip install C:\<path>\service-bootstrap\dist\service-bootstrap-<version>-py3-none-any.whl --force-reinstall
```
MacOS:
```shell
pip install <path>/service-bootstrap/dist/service-bootstrap-<version>-py3-none-any.whl --force-reinstall
```


# Upload prod
Windows:
```shell
# py -m pip install --upgrade twine
py -m twine upload dist/*
```
MacOS:
```shell
# pip install --upgrade twine
python -m twine upload dist/*
```
