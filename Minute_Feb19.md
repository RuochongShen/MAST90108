# Meeting Minutes
## Meeting Information
**Meeting Date/Time:** 19-02-2021, 11:00 am <br>
**Meeting Purpose:** Discussion <br>
**Meeting Location:** Zoom <br>
**Attendees:** Qiuhong Ke, Ruochong Shen


## Discussion Items
Index | Item | Notes | Further Details |
---- | ---- | ---- | ---- |
1 | Course requirement | Finish a short literature review in 2 or 3 days | Y |
2 | Try to use true explanation in the current model | | N |
3 | Another appproach | | Y |
4 | Attention Strategy | Use the explanation as the query of the attention in the transformer model | N |

## 1. Course requirement
**From Handbook:** 
Item | Content | Time |
---- | ---- | ---- |
A preliminary literature survey and research plan | 2 pages include: a short literature review , preliminary analysis/model development and a clear research question | by 26 Feb |
Presentation | will be assessed on their presentation skills and their ability to communicate their research to a general audience in a concise manner (15 minutes) | Week 6 - 9 (19 Apr- 16 May) |
Thesis | Theses are expected to be 30-40 pages in length, excluding references, appendices, figures, and tables. Two bound hard copies of the thesis are to be submitted | by 30 May |

## 3. Try this:
- 30dim-vector outputted by softmax; 
- Input: 30timestep, each time dim of 47 
- 30 softmax score repeat each timestep into 47 (Repeatvector (47) (softmax score))
- Transpose: 30*47
- Take the sum of feature 
- A feature vector-> mlp 
 
## Additional Notes
NA
