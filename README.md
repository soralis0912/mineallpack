# mineallpack
mineall datapack (based on TreeCaptator datapack)

[MineAll](http://forum.minecraftuser.jp/viewtopic.php?f=13&t=6874)Modの機能を[TreeCapitator](https://www.planetminecraft.com/project/treecapitator-datapack-1-13/)を参考に再現したデータパックです。

シルクタッチ、幸福、耐久力のエンチャントにも対応しています。

## 対応ブロック
* 石炭鉱石
* 鉄鉱石
* ラピスラズリ鉱石
* 金鉱石
* レッドストーン鉱石
* ダイヤモンド鉱石
* エメラルド鉱石
* ネザークォーツ鉱石
* 氷
* 氷塊
* 青氷
* グロウストーン
* 黒曜石

## インストール方法
1. このページ右上の「Clone or Download」から「Download ZIP」でZIPファイルをダウンロード
2. ダウンロードしたZIPファイルを解凍し、中身の「mineallpack-master」フォルダをマイクラのワールドフォルダの中のdatapacksフォルダの中にコピー
3. ワールドを開き、チャット欄に`[Datapack] MineAllPack has been installed`と表示されたら使用できます。
** 表示されない場合、`/function #minecraft:load`を実行するか、リソースパックの設定を変更してみてください。

## 使用方法
ツルハシで対応したブロックを破壊すると、破壊したブロックに面したブロックが連鎖して破壊されます（斜めに隣接したブロックは破壊されません）。
スニークしながら破壊すると1ブロックだけ破壊されます。
シルクタッチ付きのツルハシで破壊した場合は素材ではなく鉱石そのものがドロップします。

## 動作オプション
MineAllModと同様のオプションを用意しており、`/trigger MineAllPack`を実行して開けるオプション画面から設定できます。
オプション画面にて、角括弧（\[\])で囲まれた部分をクリックすると設定値が切り替わります（`t`キーや`/`キーでチャット入力欄を開くとクリックできるようになります）。

### 一般オプション

#### AutoCollect
onにすると、採掘したアイテムを自動的に拾います。

#### DestroyUnder
onにすると、最初に破壊したブロックより下にあるブロックもまとめて破壊します。
offにすると、最初に破壊したブロックと同じ高さか、それより上にあるブロックしか破壊しません。

#### DropGather
onにすると、採掘したアイテムが最初に破壊したブロックの座標にまとまります。
AutoCollectと同時にonにした場合はAutoCollectが優先されます。

#### Durability
ピッケルの耐久度の減り方を設定します。

* 0: 何個まとめて破壊しても、耐久度は1しか減りません。
* 1: 破壊した分だけ耐久度が減ります（耐久力のエンチャントが付いていれば、減る耐久度が少なくなります）。途中で耐久度が0になった場合でも、隣接するブロック全てが一括破壊されます。
* 2: 設定「1」と同様ですが、耐久度が0になった時点で一括破壊が止まります。

### 対象ブロックの設定
一括破壊の対象となるブロックを個別に設定できます。
（注：表示の都合上、この設定だけ別ページに分けてあります。`[一括破壊の対象ブロック設定]`をクリックしてページを切り替えて設定してください）

### 対象ツールの設定
一括破壊を有効にするツールを設定できます。木/石/鉄/金/ダイヤピッケルのそれぞれについて有効/無効を設定できます。

