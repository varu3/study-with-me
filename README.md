# study-with-me

AI が先生としてテーマを解説し、ユーザーがそれを自分の言葉で言い換え、AI がその言い換えをレビューする。これを繰り返して、テーマを自分の言葉で説明できるところまで定着させる Agent Skill。

## インストール

### Claude Code プラグインとして

```
/plugin marketplace add varu3/study-with-me
/plugin install study-with-me@study-with-me
```

### skills CLI で

```sh
npx skills add varu3/study-with-me
```

### 手動で

```sh
git clone https://github.com/varu3/study-with-me.git
ln -s "$PWD/study-with-me/skills/study-with-me" ~/.claude/skills/study-with-me
```

## 使い方

```
/study-with-me TCP
```

または「一緒に勉強しよう」「〇〇を教えて、自分の言葉でまとめるから添削して」などと話しかける。

1. AI がテーマを背景・仕組み・具体例・メリット/デメリットの流れで解説する
2. ユーザーが自分の言葉で言い換える
3. AI が正確さ・理由・抜けなどの観点でレビューし、◎ / ○ / △ で評価する
4. 次の塊へ進むか、△ の部分だけ補足して言い直す

## ライセンス

MIT
