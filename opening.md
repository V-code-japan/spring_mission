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

## くふうしてとびらのさきにすすもう @showhint
**感圧版(かんあつばん)をふむととびらがひらく**ようですが、**感圧版のうえからはなれるととじてしまいます**。
くふうして、とびらのさきにすすみましょう！
![mission2_question](/static/spring_mission2_question.gif)

