# これまでのプログラムをつかってクリアしよう！

```template
player.onChat("fl", function() {   
    agent.setAgentModeTo(AgentStates.follow)
});
player.onChat("id", function() {   
    agent.setAgentModeTo(AgentStates.idle);
});
player.onChat("ob", function() {
    agent.setAgentModeTo(AgentStates.idle);
});
player.onChat("at", function() {   
    agent.setAgentModeTo(AgentStates.attack);
});
player.onChat("br", function() {   
    agent.setAgentModeTo(AgentStates.destroy);
});
```

## これまでにつくったプログラムでめいろをこうりゃくしよう！ @unplugged
<p>これまでに作ったエージェントをうごかすプログラムをつかって、めいろをぬけだそう！</p>

## きょだいめいろ！
これまでに、したの5つのモードをつくりました。これをつかってめいろをこうりゃくしましょう！
- **たいきモード**：エージェントをそのばにとどまらせる
- **ついせきモード**：エージェントがうしろをついてくる
- **カメラモード**：エージェントがそらからめいろをみる
- **こうげきモード**：エージェントがちかくのモンスターをこうげきする
- **スポナーはかいモード**：エージェントがちかくのスポナーブロックをこわす