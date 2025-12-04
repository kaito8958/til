# 投稿編集チェックボックスが保持されない問題を修正

JSON カラムに "1" のような文字列で ID が保存されていたため、
ビュー側で整数 1 と比較すると一致せず、チェックが外れて見えていた。

`Post` モデルで getter を上書きし、
読み出し時に常に整数化するように修正。

```ruby
def genre_ids
  super&.map(&:to_i)
end

def looking_for_skill_ids
  super&.map(&:to_i)
end

