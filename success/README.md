# README

これは成功例。  
構造や`__init__.py`などは`dismiss`と同一。


`pip extra`を使用してライブラリ時には依存関係がインストールされないようにしている  


## 注意点

### 注意点１
`poetry`を使った時と`pip install -e`を使った時で子パッケージの編集可能パッケージのパスが変わること。  
- poetryの場合
  - `<module 'suba' from 'pkgs/suba/suba/__init__.py'>`
- pipの場合
  - `<module 'suba' from '.venv/lib/python3.10/site-packages/suba/__init__.py'>`

## 注意点2

poetryのエクストラパッケージの設定方法は、まず`--optional`でインストールして、`[tool.poetry.extras]`を直接作成して内部を編集する。  
詳細は [suba/pyproject.toml](suba/pyproject.toml) を確認すること
