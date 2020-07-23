# grandblueCalculator
https://shin1127.github.io/grandblueCalculator

# Introduction
ソーシャルゲーム『グランブルーファンタジー』のダメージ計算機。

# Background
~~所属しているコミュニティで、メンバーからキャラクターや装備をヒアリングするなどして、代わりに予測ダメージを演算するのが面倒になったので作った。  
JSを含むフロントサイドの勉強にもなると考えた。~~  
よくよく考えてみると、  
「計算方法を検索するのが面倒」「計算方法がそもそも分からない」  
というユーザーに応える形でサービスを作ったことになる、という認識を得た。

# Things I learned

-  全体としては中央寄せだがこの部分は左寄せをしたい、というときはCSSでdisplay: inline-blockを使う。
-  少しでもテクニカルしようと思い、JSONファイルに定数を格納して使うということも考えたが正直面倒くさい。新しい要素を追加するとき、変更すべき箇所が少なくなるように設計するのが一番よいと感じた。
-  ブラウザベースで実装しようという場合でも、はじめにコンソールベースで実装する（しようとする）と、完成までの道のりが分かりやすい。
-  入力ボックスの中身を空にする == 入力ボックスを""で書き換える
-  ラジオボタンの入力状況でも、チェックボックスでも入力ボックスでも、JSファイル内で値を取得するときの流れはほぼ同じ
-  constで最初に値を宣言するのいらないのではないか（一度しか利用しない上に可変ではない）
-  レスポンシブデザインを考えるときはGoogleChromeの拡張機能Responsiv Viewerが便利だった（ただしローカルのファイルは使えないため、Githubpagesにアップロードしておく必要がある）
-  テキストボックスで整数の入力だけを受け付けたい　->  <input type="number" min="0">
