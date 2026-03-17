# とびらのさきにすすもう！ @showdialog
じどうでしまるとびらのさきにすすもう！
``` template
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
## くふうしてとびらのさきにすすもう @fullscreen
**感圧版(かんあつばん)をふむととびらがひらく**ようですが、**感圧版のうえからはなれるととじてしまいます**。
くふうして、とびらのさきにすすみましょう！
![complete1](https://vcode-esia.com/images_for_world_data/2026_spring/spring_mission1_complete.gif)

