# エージェントといっしょにモンスターをたおそう！

```template
player.onChat("fl", function() {   
    agent.setAgentModeTo(AgentStates.follow)
});
player.onChat("id", function() {   
    agent.setAgentModeTo(AgentStates.idle);
});
player.onChat("ob", function() {
    agent.setAgentModeTo(AgentStates.observe);
});
player.onChat("at", function() {});
player.onChat("br", function() {});
```

## エージェントをつかってめいろをこうりゃくしよう！ @unplugged
<p>エージェントの**こうげきモード**、**スポナーはかいモード**をつかって、めいろをぬけだそう！</p>
<br></br>
<img src="https://vcode-esia.com/images_for_world_data/2026_spring/attack_mode.gif" width=50%><img src="https://vcode-esia.com/images_for_world_data/2026_spring/destroy_mode.gif" width=50%>

## ここからのめいろは・・・
こんどのめいろは、**モンスターべや**があります！

- へやのまんなかにある**スポナーブロック**をこわすまで、モンスターがわきでてくる
- スポナーブロックは、**エージェント**か**ネザライトのつるはし**でこわせる

**モンスターをよけたり、スポナーブロックをこわしたりしながら**めいろからだっしゅつしよう！

## こうげきモードをつかおう
エージェントには**こうげきモード**があるようです。
これをつかえば、**ちかくにいるモンスターをじどうでこうげきする**ことができます！
![attack mode](https://vcode-esia.com/images_for_world_data/2026_spring/attack_mode.gif)

## プログラミングしよう
1. `||agent.エージェント||`から、`||agent.エージェントをつぎのモードにする||`をとりだす
2. `||player.チャットコマンド at を入力(にゅうりょく)した時||`にはめこむ
3. モードを**こうげきモード**にする

```block
player.onChat("at", function() {   
    agent.setAgentModeTo(AgentStates.attack);
});
```

## スポナーはかいモードをつかおう
モンスターは**スポナーブロック**があるかぎりむげんにスポーンするようです・・・。
エージェントときょうりょくしてこわしましょう！
スポナーブロックをこわせば、**そのへやにいるモンスターをすべてたおせます！**
![destroy mode](https://vcode-esia.com/images_for_world_data/2026_spring/destroy_mode.gif)

## プログラミングしよう
1. `||agent.エージェント||`から、`||agent.エージェントをつぎのモードにする||`をとりだす
2. `||player.チャットコマンド br を入力(にゅうりょく)した時||`にはめこむ
3. モードを**スポナーはかいモード**にする

```block
player.onChat("br", function() {   
    agent.setAgentModeTo(AgentStates.destroy);
});
```

## めいろのちずをつくろう！
これまでにつくったプログラムをつかって、**ワークシートにちずをかんせいさせよう！**

👍**ポイント**👍
それぞれのモード中のエージェントは、**かべやとびらをすりぬける**ことができます！
さきにモンスターべやかどうかわかっていれば、**とびらのそと**からこうげきやスポナーはかいができるかも・・・？
![wall hack](https://vcode-esia.com/images_for_world_data/2026_spring/wall_attack.png)