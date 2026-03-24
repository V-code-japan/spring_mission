# これまでのプログラムをつかってクリアしよう！

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

## めいろのなかのめいろをぬけだそう！
このめいろには、**めいろべや**があるようです。
めいろべやは、**ちいさくなるとすすむことができます**。
めいろべやのなかでおおきくなると、**まわりがみわたせる**かわりに**そのばからうごけなくなります**。
うまくつかいわけましょう！
![maze in maze](https://vcode-esia.com/images_for_world_data/2026_spring/maze_in_maze.png)

## ちいさくなると・・・
**うちでのこづち**をつかうと・・・
- **30びょうかんちいさくなる**
- もういちどつかうと、30びょうよりみじかくてももとにもどる
- めいろべやをとおることができる
- **エージェントのカメラモードがつかえなくなる**
![mini](https://vcode-esia.com/images_for_world_data/2026_spring/mini_sized.png)