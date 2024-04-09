# item_modifier-enchant_with_levels
item_modifierの1項目であるenchant_with_levelsに関するサンプルです。

~詳しくはブログ記事『[]()』を参考にしてください。~<br>
現在執筆中

<h3>概要</h3>

エンチャントを付与することのできるitem_modifierの項目です。<br>
レベルを指示するため、どの程度のエンチャントが付与されるのかを調整できます。

エンチャントテーブルを用いたエンチャントを行う際のイメージを想定すれば、概ね合っています。

<h3>使い方</h3>

データパック導入後、ワールドに入ることで鉄のツルハシを3つ付与されます。

このツルハシを手に持った状態で

```copy
/item modify entity @s weapon.mainhand sample:enchant_with_levels_lv30
```

と実行することで、enchant_with_levelsを用いたエンチャント付与が行えます。

---

ルートテーブルに組み込むことも可能で

```copy
/loot give @s loot sample:enchant_with_levels_trident
```

と実行すると、エンチャントが付与されているトライデントが入手可能です。

また

```copy
/loot give @s loot sample:enchant_with_levels_emerald
```

と実行するとエメラルドが付与されますが、これはエンチャントテーブルを用いたエンチャントとしては不適切なため、エンチャントが施されないまま付与されます。
