# university-assignments
大学の講義・演習で作成したプログラム

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
touch "$SUBJECT/$ASSIGNMENT/README.md"
touch "$SUBJECT/$ASSIGNMENT/memo.md"
```

### Directory Structure

```text
SUBJECT/
├── README.md
└── ASSIGNMENT/
    ├── README.md
    ├── memo.md
    ├── src/
    └── results/
```

### Naming Rules

- `SUBJECT`：科目名（英語表記）
- `ASSIGNMENT`：課題名（英語表記）
- `src/`：ソースコード
- `results/`：実行結果・出力ファイル
- `memo.md`：実装時のメモ・考察