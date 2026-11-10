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
```

### Directory Structure

```text
university-assignments/
├── README.md
└── SUBJECT/
    ├── README.md
    └── ASSIGNMENT/
        ├── memo.txt
        ├── src/
        └── results/
```

### Naming Rules

- `SUBJECT`：科目名（英語表記）
- `ASSIGNMENT`：課題名（英語表記）
- `src/`：ソースコード
- `results/`：実行結果・出力ファイル
- `memo.txt`：実装時のメモ・考察
- `README.md`：科目ごとの課題管理・説明