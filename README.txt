# Kulack's changes

* Added --print=s option so that just the HTTP status can be printed

# To Build
```
brew install httpie

git clone git@github.com:httpie/httpie.git
cd httpie

python3 -m venv venv
. ./venv/bin/activate
pip install -r requirements-dev.txt

python setup.py install
DST=/usr/local/Cellar/httpie/*/libexec/bin
cp venv/bin/http* $DST
```