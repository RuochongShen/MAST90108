# Meeting Minutes
## Meeting Information
**Meeting Date/Time:** 15-01-2021, 11:00 am <br>
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

Progress: one version of the transformer code is fixed and training accuracy is nearly 1 after 20 epochs; still need to have a better understanding on the code.

**To do:** 
 - Use the formal split instead of the current split and evaluate by cross-validation;
 - Use concat one time to the time steps and take only one action as the output;
 - Read the paper and try to find and read the sample code on classification tasks to understand transformer;
 - Maybe try to use word embedding and take the average, and then concat the time to get the input of the decoder.
 
## Additional Notes
NA
