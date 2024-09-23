## settings.json設定

### VSCODE拡張
以下のVSCODE拡張をインストールする
- Black Formatter	"ms-python.black-formatter"
- Flake8	"ms-python.flake8"
- isort	"ms-python.isort"

をインストール

### pip install
requirements-dev.txtに
```
black
flake8
isort
```
を加えて

```
$ pip insatll -r requirements-dev.txt
```
