# Meeting Minutes
## Meeting Information
**Meeting Date/Time:** 26-02-2021, 11:00 am <br>
**Meeting Purpose:** Discussion <br>
**Meeting Location:** Zoom <br>
**Attendees:** Qiuhong Ke, Ruochong Shen


## Discussion Items
Index | Item | Notes | Further Details |
---- | ---- | ---- | ---- |
1 | Change t and gt_expl |  | Y |
2 | Attention Strategy: Investigate different attention methods | | Y |
3 | Demo sampling instead of probability distribution | | Y |
4 | Test with predicted explanation class but not gt_expl |  | Y |

## 1. 
- t: 1-300 intead of [1,3,5,7,10:60:10]; testing with points like [1,3,5,7,10:60:10,90:300:30];
- try different input: with/without last action/gt_expl;
- try to remove true t second;
- try to test with gt_expl.

## 2. Attention Strategy
- simple attention discussed last week: 
  - 30dim-vector outputted by softmax
  - Input: 30timestep, each time dim of 47
  - 30 softmax score repeat each timestep into 47 (Repeatvector (47) (softmax score))
  - Transpose: 30*47
  - Take the sum of feature
  - A feature vector-> mlp
- investigate different attention methods

## 3. Try this:
- feature_vec + real t sec -> expl; feature_vec + expl -> prob;
- use demo sampling (by gamble softmax or turn prob to one-hot of the action)
 
## 4. Train separately:
- t: 1:300 (same with 1)
- feature_vec + t -> expl; feature_vec + expl -> action
 
## Additional Notes
NA
