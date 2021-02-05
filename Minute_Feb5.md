# Meeting Minutes
## Meeting Information
**Meeting Date/Time:** 05-02-2021, 11:00 am <br>
**Meeting Purpose:** Discussion <br>
**Meeting Location:** Zoom <br>
**Attendees:** Qiuhong Ke, Ruochong Shen


## Discussion Items
Index | Item | Notes | Further Details |
---- | ---- | ---- | ---- |
1 | Fix the current approaches |  | Y |
2 | Try the similar approaches on TCN and LSTM | | Y |
3 | Try two new approaches | | Y |

## 1. Fix the current approaches
**Content:** 
- Explanation class: size 6 -> 5 (remove None);
- Approach name: try to make them clear;
- Use cross validation for testing: average on 4 splits instead of 1;
- Fix bugs: approaches should have high accuracy for small t - maybe 95% for t=1;

## 2. Try the similar approaches on TCN and LSTM
**Note:**
- Try to figure out why the explanations are not improving the accuracy of the action anticipation;

## 3. Try two new approaches: train jointly. (Optional)
- Input -> Action -> Explanation -> Action;
3 cross entropy + 1 KL divergence on the 2 action outputs.

- Input -> Action -> Explanation -> Action -> Explanation;
4 cross entropy + 2 KL divergence on the 2 action outputs and the 2 explanation class outputs.
 
## Additional Notes
NA
