# エージェントをうごかしてだっしゅつしよう！
```template
player.onChat("fl", function () {
	
})
player.onChat("go", function () {
	
})
player.onChat("id", function () {
	
})
```
```block
player.onChat("fl", function() {   
    agent.setAgentModeTo(AgentStates.follow)
});
player.onChat("id", function() {   
    agent.setAgentModeTo(AgentStates.go);
});
player.onChat("go", function() {
    agent.move(UP, 4);
    agent.move(FORWARD, 2);
    agent.move(DOWN, 4);
});
```

## エージェントをうごかそう @unplugged
<p>エージェントをスイッチまでいどうさせよう！</p>
<br></br>
<img src="https://vcode-esia.com/images_for_world_data/2026_spring/spring_mission1_complete.gif" width=50%><img src="https://vcode-esia.com/images_for_world_data/2026_spring/spring_mission1_complete2.gif" width=50%>

## ついせきモード
`||agent.エージェント||`を**ついせきモード**にすると、エージェントが**プレイヤーのあとをついてあるきます**。
このモードをつかって、**エージェントをとびらのまえまでうごかしましょう！**


## プログラミングしよう
- `||agent.エージェント||`から、`||agent.エージェントをつぎのモードにする||`をとりだす
- `||player.チャットコマンド fl を入力(にゅうりょく)した時||`にはめこむ
```block
player.onChat("fl", function() {   
    agent.setAgentModeTo(AgentStates.follow);
});
```

## ついせきをとめる
ついせきモードをやめるには、エージェントを**たいきモード**にします。
チャットで**id**とにゅうりょくしたら、たいきモードになるようにプログラミングしましょう！

## プログラミングしよう
- `||agent.エージェント||`から、`||agent.エージェントをつぎのモードにする||`をとりだす
- `||player.チャットコマンド id を入力(にゅうりょく)した時||`にはめこむ
- モードを**たいきモード**にする
```block
player.onChat("id", function() {   
    agent.setAgentModeTo(AgentStates.idle);
});
```
## エージェントをとびらのまえまでうごかそう！ @showhint
これでエージェントがついてくるようになりました！
右下の**▶**(じっこうボタン)をおして、したのようににゅうりょくしてみましょう。
- **fl**: エージェントがプレイヤーのあとをついてくる
- **id**: エージェントがそのばにとまる

⚠️**ちゅうい**⚠️
エージェントをとびらのまえまでうごかせたら、もういちど**C**をおして、この画面をひらきましょう。

![complete](https://vcode-esia.com/images_for_world_data/2026_spring/spring_mission1_complete.gif)



## エージェントをスイッチまでうごかす
つぎに、チャットで**go**とにゅうりょくしたら、**エージェントがスイッチまでいどうする**ようにしましょう。

## プログラミングしよう
- `||agent.エージェント||`から、`||agent.エージェントを 前(まえ) に 1　ブロック移動(いどう)させる||`をとりだす
- `||player.チャットコマンド go を入力(にゅうりょく)した時||`にはめこむ

おなじようにして、ブロックを**３つ**ならべましょう。

## うごかすむきときょりをきめる
つぎに、エージェントをうごかす**むき**と**きょり**をきめましょう！

1. 上(うえ)に４ブロック
2. 前(まえ)に２ブロック
3. 下(した)に４ブロック

となるように、むきときょりをせっていしましょう。
```block
player.onChat("go", function() {
    agent.move(UP, 4);
    agent.move(FORWARD, 2);
    agent.move(DOWN, 4);
});
```

## エージェントをスイッチまでうごかそう
エージェントをスイッチまでうごかして、へやからでられるようにしましょう。
右下の**▶**(じっこうボタン)をおしたら、したのようにしましょう。

1. **エージェントのえ**を**みぎクリック**して、エージェントがとおれるようにする
2. チャットで**go**とにゅうりょくする

![complete2](https://vcode-esia.com/images_for_world_data/2026_spring/spring_mission1_complete2.gif)



