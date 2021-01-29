# Meeting Minutes
## Meeting Information
**Meeting Date/Time:** 29-01-2021, 3:00 pm <br>
**Meeting Purpose:** Discussion <br>
**Meeting Location:** Zoom <br>
**Attendees:** Qiuhong Ke, Ruochong Shen


## Discussion Items
Index | Item | Notes | Further Details |
---- | ---- | ---- | ---- |
1 | Further coding task on anticipation |  | Y |

## 1. Further coding task on anticipation
**Content:** 
Purpose: Use the time-conditioned transformer model and train the following task: 
- input:  observation features; output: the future action + the type of explanation
- input:  type of explanation + observation features; output: the future action
- output the action class, and then use the action class to explain First learn transformer

**Progress:** 
From last week:
- Evaluate the results for each anticipation time 1 3 5 7 10:10:60.
- Try out the following approaches (training jointly):
  1. Build one transformer model and take both the class of the explanation and the anticipated action as the output;
  2. Build two transformer models: input -> explanation class; input + explanation class -> anticipated action;
  3. Build two transformer models: input -> anticipated action; input + anticipated action -> explanation class;
  And compare the results.
- Try other models on CV: advanced type of transformer models, TCN and LSTM. Build a table or something to compare the results.

The result is not ideal: the explanations are not improving the accuracy of the action anticipation.

**To do:** 
Try to both train jointly and separately:
- use action order (index) instead of the real time;
- only keep one action for each action segment instead of 1 timestep per second (e.g. by masking: difference with shifting sequence);
- try lstm first to see the results.

 
## Additional Notes
NA
