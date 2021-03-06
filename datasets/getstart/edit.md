<Section>
# FBE チュートリアル

ここではFBEにを使いこなすためのチュートリアルを
紹介します。

## フローチャートを編集する

思い描くフローチャートを構築できるように
ここではフローチャートの編集方法を学びます。

</Section>

<Section>

## FBEにアクセスする

下のボタンからFBEにアクセスしましょう！

[FBEを開く](https://fbe.vercel.app/)

また、すでにフローチャートがある場合は
 `左上のメニューボタン(3本線が目印)`→`新規作成` をクリックして画面をまっさらにしておきましょう。

</Section>

<Section>

## 操作の規則

FBEを操作するうえで以下の4点を覚えておきましょう。知らない操作や忘れてしまった操作を探すときに役立つはずです。

<Blue>
- 記号・フローに関する操作（記号などの削除など）は パソコンでは画面右の、スマホでは画面下の**サイドバー**から操作する

- 記号やフローを操作するときは、おおむね**①記号やフローを選択する**,**②サイドバーから操作**する。

- 選択中の記号やフローは**青色**

- フローチャート全体に関する操作（フローチャートを保存するなど）は 画面左上の（パソコン・スマホ共通）の**メニューボタン**から操作する
</Blue>

</Section>

<Section>

## フロー

FBEでは流れ図記号をフローの中に追加して作成していきます。
（今はよくわからなくてもとりあえず読み進めてみましょう）

フローは

<HowTo>
- サイドバーのメニューを開くボタン
- フローを追加
</HowTo>

と追加することができます。

</Section>

<Section>

## 記号の種類

このチュートリアルを作成した時点では、FBEでは7種の記号を用意しています。

<Alert>
**あなたはこれらを覚える必要は一切ありません！**記号について詳しく知りたくなった時に見返しに来てください。
</Alert>

|記号|役割|重要度|
|---|---|---|
|端子|プログラムの**はじめ**や**おわり**を示します|☆☆☆|
|計算|数字などを計算をして**変数に代入**します|★★★|
|繰り返し（2種類）|処理を**繰り返し**ます|★★★|
|分岐（2種類）|条件によって処理を**分岐**します|★★★|
|データ|データを**入力**したりデータを**表示**したりします|★★☆|
|準備|**配列**などを準備します。|★☆☆|
|定義済み処理|別のフローや特別な処理を呼び出します。|★☆☆|

## 記号の基本操作

### 記号の追加

記号は

<HowTo>
- フローチャート上の＋ボタンをクリック
- 追加したい記号の種類をクリック
</HowTo>

と追加できます。また追加後は自動的に追加した記号が選択されます。

### 記号の削除

間違えて記号を追加してしまった時などは以下のように記号を削除することができます。

<HowTo>
- 記号をクリックして選択（記号が青色になります）
- サイドバーのメニューを開く
- 記号を削除
</HowTo>


</Section>

<Section>

## 面積計算プログラムを作る

三角形の面積を計算するプログラムを作ってみましょう。

はじめにプログラムの処理を箇条書きにしてみます

```
高さを入力

底辺を入力

面積を求める（高さ*底辺/2）

面積を表示する
```

これをフローチャートにしてみましょう。

上の4つの処理はそれぞれ

<Blue>
- 〇〇を入力 → データ記号
- 〇〇を求める → 計算記号
- 〇〇を表示する → データ記号
</Blue>

を使って表現できます。（記号の種類の表を参考に）

それではそれぞれフローチャートにしてみてください。

---

### フローを追加

まずはフローを追加します。

<HowTo>
- サイドバーのメニューを開くボタン
- フローを追加
</HowTo>

### "高さを入力"を追加

次に「**高さを入力**」を追加してみましょう。

先ほど確認したとおり、 "〇〇を入力" の処理は
データ記号を使うことで表現できますので、

<HowTo>
- フローチャートの＋ボタン
- データ記号
</HowTo>

とデータ記号を追加しましょう。

データ記号は追加できました！ですが、データ記号には"変数を出力"
と表示されてしまっています。
今回は**高さ**を**入力**したいのでその二つを設定しましょう。

記号により詳しい設定を加えたいときは記号に**オプション**を設定します。
オプションを設定することですべての記号で必要なものがあらかじめ設定されていますが、
必要に応じて変更していくことで細かく設定が可能です。

記号を選択しているとサイドバーのオプションのあたりに**選択中の記号のオプション**が表示されます。記号を選択していない場合は記号を選択しましょう。（選択したデータ記号が**青色**になっているはずです）

データ記号には"タイプ"オプションと"対象"オプション,"数字を入力"オプションがあります。

"タイプ"オプションは**データを入力するのか、データを出力（表示）するのか**を選択します。デフォルトでは出力になっているので**入力**に変更しましょう。出力となっているところをクリックして**キーボード入力**を選択します。

"対象"オプションは**何を入力するのか**を指定します。今回は高さを設定したいので高さと入力します。

"数字を入力"オプションは入力する値が数字ならばチェックボックスを入れます。高さは数値になるはずなので**チェックを入れておきましょう**。

<!-- 全オプション設定後の画像 -->

これで"高さを入力"データ記号を設定できました。

### "底辺を入力"を追加

"底辺を入力"も"高さを入力"と同じように追加することもできますが、
ここで**記号の複製**を使ってみましょう。

<HowTo>
- "高さを入力"データ記号を選択した状態でサイドバーのメニューを開く
- 複製
</HowTo>

で記号を複製できます！

下に複製されました。下のデータ記号を選択して"対象"オプションを
**底辺**に変更します。

これで"底辺を入力"データ記号も設定ができました！

### "面積を求める"を追加

これまではデータ記号をフローチャートに追加してきました。
今度は"面積を求める"計算記号を追加しましょう。

<HowTo>
- "底辺を入力"の下の＋ボタン
- 計算
</HowTo>

を選択して、計算記号を追加します。

計算記号には"式","代入先変数"オプションがあります。

"式"オプションには計算の内容を指定します。
面積は`高さ*底辺/2`で求めることができるので、
"式"オプションには**高さ*底辺/2**を指定します。

<Alert>
FBEでは掛け算を **＊(アスタリスク)** , 割り算を **/(スラッシュ)** で指定します。×や÷を使わないように注意してください。 
</Alert>

"代入先変数"オプションには計算結果を代入する変数を指定します。
計算結果は面積に設定したいので"代入先変数"オプションに
**面積**と指定します。

これで"面積を求める"計算記号も設定ができました！

### "面積を表示"を追加

データ記号を使って"面積を表示"を追加しましょう。

<HowTo>
- "高さ*底辺/2 → 面積"記号の下の＋ボタン
- データ
</HowTo>

でデータ記号を追加します。

今回は**面積** を **表示**したいので

- "タイプ"オプションは出力
- "対象"オプションは面積

を指定しましょう。

<Success>
ここまで設定できればあなたのフローチャートは完成しました！お疲れさまでした。
</Success>

この章を終えたあなたはフローチャートの編集の基礎を学びました。基礎といっても大抵のフローチャートの作成は今回の知識のみで十分可能なことが多いです。自信を持ってください！！！

次以降のページでフローチャートを実行したり、フローチャートを保存したりできます。

[フローチャートを実行のチュートリアル](/getstart/execute)




</Section>


