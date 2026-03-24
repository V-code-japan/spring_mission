# エージェントをつかってめいろをこうりゃくしよう！

```template
player.onChat("fl", function() {   
    agent.setAgentModeTo(AgentStates.follow)
});
player.onChat("id", function() {   
    agent.setAgentModeTo(AgentStates.idle);
});
player.onChat("ob", function() {});
```

## エージェントをつかってめいろをこうりゃくしよう！ @unplugged
エージェントの**カメラモード**をつかって、めいろをぬけだそう！
![camera mode](https://vcode-esia.com/images_for_world_data/2026_spring/camera_mode.gif)

## めいろをだっしゅつしよう
**めいろにとじこめられてしまいました・・・**ゴールを見つけましょう！

- **へやからでるとびら**をあけると、**カギ**を１つつかう
- カギがないじょうたいでへやからでるとびらをあけると、**スタートにもどされてしまう**

**エメラルドブロックのうえにたって**めいろからだっしゅつしよう！
![goal](https://vcode-esia.com/images_for_world_data/2026_spring/emerald.png)

## カメラモードをつかおう
エージェントには**カメラモード**があるようです。
これをつかえば、**めいろをうえからみる**ことができます！
カメラモードをつかいながらめいろを探索(たんさく)して、**めいろのちずをつくりましょう！**
![camera mode](https://vcode-esia.com/images_for_world_data/2026_spring/camera_mode.gif)

## プログラミングしよう
1. `||agent.エージェント||`から、`||agent.エージェントをつぎのモードにする||`をとりだす
2. `||player.チャットコマンド bl を入力(にゅうりょく)した時||`にはめこむ
3. モードを**カメラモード**にする

```block
player.onChat("ob", function() {   
    agent.setAgentModeTo(AgentStates.observe);
});
```

## めいろのちずをつくろう！
プログラミングした**カメラモード**をつかって、**ワークシートにちずをかんせいさせよう！**
カメラモードをかいじょしたいときは、チャットで**fl**とにゅうりょくして、エージェントを**ついせきモード**にしましょう。
