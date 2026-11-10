# university-assignments

大学の講義・演習で作成したプログラムを管理するリポジトリ．

## Directory Creation

### Create a New Assignment

科目名と課題名を指定して，ディレクトリを作成する．

```bash
# Set directory names
SUBJECT="information-security"
ASSIGNMENT="caesar-cipher"

# Create directories
mkdir -p "$SUBJECT/$ASSIGNMENT"/{src,results}

# Create files
touch "$SUBJECT/README.md"
touch "$SUBJECT/$ASSIGNMENT/memo.txt"
touch "$SUBJECT/$ASSIGNMENT/requirements.txt"
```

### Directory Structure

```text
university-assignments/
├── README.md
└── SUBJECT/
    ├── README.md
    └── ASSIGNMENT/
        ├── memo.txt
        ├── requirements.txt
        ├── src/
        └── results/
```

### Naming Rules

- `SUBJECT`：科目名（英語表記）
- `ASSIGNMENT`：課題名（英語表記）
- `src/`：ソースコード
- `results/`：実行結果・出力ファイル
- `memo.txt`：実装時のメモ・考察
- `requirements.txt`：Pythonの外部ライブラリとバージョン
- `README.md`：リポジトリ全体または科目ごとの説明

## Python Environment

### Install Dependencies

課題ディレクトリに移動して，必要なライブラリをインストールする．

```bash
pip install -r requirements.txt
```

### Add Dependencies

新しい外部ライブラリを使用する場合は，`requirements.txt` にライブラリ名とバージョンを記載する．

```text
numpy==2.2.0
```

※ Python標準ライブラリのみを使用する場合，`requirements.txt` は空でよい．