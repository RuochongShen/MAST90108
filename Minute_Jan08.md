# Meeting Minutes
## Meeting Information
**Meeting Date/Time:** 08-01-2021, 11:00 am <br>
**Meeting Purpose:** Discussion <br>
**Meeting Location:** Zoom <br>
**Attendees:** Qiuhong Ke, Ruochong Shen


## Discussion Items
Index | Item | Notes | Further Details |
---- | ---- | ---- | ---- |
1 | Annotation task | Finished; No need to add the goal of the video into the explanation. | N |
2 | Further coding task on anticipation |  | Y |

## 1. Further coding task on anticipation
**Content:** Use the time-conditioned transformer model and train the following task: 
- input:  observation features; output: the future action + the type of explanation
- input:  type of explanation + observation features; output: the future action
- output the action class, and then use the action class to explain First learn transformer

Take the observation as a sequence with 30 timesteps; take 47 actions as an one-hot variable; Make the time as a scalar and put it in the embedding layer and output the vector of the time; Concat time vector with the feature output of the sequence.

**To do:** 
 - First learn to use the transformer model and output without explanation
 - Construct matrix of probability of transform from one  action  to the next action: 47*47*3 (next action, next second action, next third action)

## Additional Notes
NA
