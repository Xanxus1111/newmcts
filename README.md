# newmcts
AIG assignment1

In test.java file add those lines then it works.

```
import players.newmcts.newMCTSParams;
import players.newmcts.newMCTSPlayer;



newMCTSParams newMCTSParams = new newMCTSParams();
players.add(new newMCTSPlayer(seed, playerID++, new newMCTSParams()));
```

In run.java file 

```
import players.newmcts.newMCTSParams;
import players.newmcts.newMCTSPlayer;

case 6:
  newMCTSParams newmctsParam = new newMCTSParams();
  newmctsParam.stop_type = newmctsParam.STOP_ITERATIONS;
  newmctsParam.num_iterations = 200;
  newmctsParam.rollout_depth = 12;

  newmctsParam.heuristic_method = newmctsParam.CUSTOM_HEURISTIC;
  p = new newMCTSPlayer(seed, playerID++, newmctsParam);
  playerStr[i-4] = "newMCTS";
  break;
```
