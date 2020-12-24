# チーム開発 Ruby 課題（応用）

## 教材のご案内

- 逆転教材のテキスト教材
  - オブジェクト指向
- ドラクエ風ゲームプログラムを作ってみよう！
  - [https://www.techpit.jp/courses/ruby-dragon-quest/lectures/12476434](https://www.techpit.jp/courses/ruby-dragon-quest/lectures/12476434)
  - 無料の範囲内で課題を解く上で必要となる内容を学習できます

## 回答方法について

- Ruby 課題（基礎）を参照下さい

## Q17. 次の User クラス 内に info メソッドを追加し，期待する出力結果になるようにして下さい。

```
class User

# コードを追加

end

user1 = User.new(name: "神里", age: 32, gender: "男")
user2 = User.new(name: "あじー", age: 32, gender: "男")

user1.info
puts "-------------"
user2.info
```

期待する出力結果

```
名前：神里
年齢：32
性別：男
-------------
名前：あじー
年齢：32
性別：男
```

## Q18. 年齢を用いた場合分けを利用して，期待する出力結果になるような User クラスを作成して下さい。

```
# コードを追加

user1 = User.new(name: "あじー", age: 32)
user2 = User.new(name: "ゆたぼん", age: 10)

puts user1.introduce
puts user2.introduce
```

期待する出力結果

```
こんにちは，あじーと申します。宜しくお願いいたします。
はいさいまいど〜，ゆたぼんです！！！
```

## Q19. 次のコードはエラーが出ます。期待する出力結果となるようにコードを修正して下さい。

```
class Item
  def initialize(name)
    @name = name
  end
end

book = Item.new(name: "ゼロ秒思考")
puts book.name
```

期待する出力結果

```
ゼロ秒思考
```

## Q20. 次の仕様を満たした上で，期待する出力結果になるようにコードを追加して下さい。

- 年齢区分は，幼児(0〜5 歳)，子供(6〜12 歳)，成人(13〜64 歳)，シニア(65〜120 歳)の 4 パターンとします。（この範囲外の年齢については対処しなくて OK です）

```
class User

  # コードを追加

end

class Zoo

  # コードを追加

end

zoo = Zoo.new(name: "旭山動物園", entry_fee: { infant: 0, children: 400, adult: 800, senior: 500 })

users = [
  User.new(name: "たま", age: 3),
  User.new(name: "ゆたぼん", age: 10),
  User.new(name: "あじー", age: 32),
  User.new(name: "ぎん", age: 108)
]

users.each do |user|
  zoo.info_entry_fee(user)
end
```

期待する出力結果

```
たまさんの入場料金は 0 円です。
ゆたぼんさんの入場料金は 400 円です。
あじーさんの入場料金は 800 円です。
ぎんさんの入場料金は 500 円です。
```
