# Meeting Minutes
## Meeting Information
**Meeting Date/Time:** 23-12-2020, 10:30 am <br>
**Meeting Purpose:** Discussion <br>
**Meeting Location:** Zoom <br>
**Attendees:** Qiuhong Ke, Ruochong Shen


## Discussion Items
Index | Item | Notes | Further Details |
---- | ---- | ---- | ---- |
1 | Presentation | | Y |
2 | Annotation task to do | Important | Y |
3 | Regular meeting | Every Friday from 8th Jan at 11am; can be adjusted | N |

## 1. Presentation
**Content:** Make a slide and have some discussion on "Learning to Explain with Complemental Examples": too much details included but only a general idea required. <br>
**To do:** 
 - Roughly read "How Can I Explain This to You? An Empirical Study of Deep Neural Network Explanation Methods" to get some general ideas on explanation models on action recognition; Maybe a presentation on it later on. 
 - List of paper to read:
 
Title |
---- |
Attention Branch Network: Learning of Attention Mechanism for Visual Explanation |
Multimodal Explanations by Predicting Counterfactuality in Videos |
Teaching Categories to Human Learners with Visual Explanations |
Multimodal Explanations: Justifying Decisions and Pointing to the Evidence |
Explainable Object-induced Action Decision for Autonomous Vehicles |
How Does Noise Help Robustness? Explanation and Exploration under the Neural SDE Framework |
Interpretable and Fine-Grained Visual Explanations for Convolutional Neural Networks |
SAM: The Sensitivity of Attribution Methods to Hyperparameters |
SCOUT: Self-aware Discriminant Counterfactual Explanations |
Towards Global Explanations of Convolutional Neural Networks with Concept Attribution |
Towards Visually Explaining Variational Autoencoders |
Attribution in Scale and Space |
Axiomatic Attribution for Deep Networks |
Explainability Methods for Graph Convolutional Neural Networks |
VQA with No Questions-Answers Training |

**Notes:** NA

## 2. Annotation task to do
**Content:** For the two datasets: 

Dataset | No. of videos | Link | Paper |
---- | ---- | ---- | ---- |
breakfast | 1700 | https://serre-lab.clps.brown.edu/resource/breakfast-actions-dataset/ <br> Download: https://mega.nz/file/O6wXlSTS#wcEoDT4Ctq5HRq_hV-aWeVF1_JB3cacQBQqOLjCIbc8 | https://serre-lab.clps.brown.edu/wp-content/uploads/2014/05/paper_cameraReady-2.pdf |
gtea | 28 | http://cbs.ic.gatech.edu/fpv/ | |

Some annotations could be done. <br>
Paper: https://openaccess.thecvf.com/content_CVPR_2019/papers/Ke_Time-Conditioned_Action_Anticipation_in_One_Shot_CVPR_2019_paper.pdf <br>
Data files: some .txt files like "P03_cam01_P03_cereals.txt" that includes many action labels of a video (ordered by time), with lots of "SIL" or "background" at the beginning and the end of the file. <br>
For each dataset, we can take part of each video as the observation to anticipate its future. For example, given 10% of a video in the Breakfast dataset, one could be interested in the action that's going to be performed after 1 sec, 2 sec, ..., which may be done by a deep network, as well as the reason why that deep learning model makes that prediction. That is, long-term prediction with explanation is an interesting topic to do research on. <br>
So as a first step, we would like to annotate the data with the action labels after t seconds as well as an explanation using the last two actions, the last second action of the observation and the goal of the person in a video. The parial percentage and time t are listed below.

Dataset | Partial Percentage of a video as Observation | Time t after the observation (sec) |
---- | ---- | ---- |
breakfast | 10%, 20%, ..., 90% | 1, 3, 5, 7, 10, 20, 30, 40, 50, 60 |
gtea | 1%, 2%, ...., 99% | 1, 2, ..., 20 |

**To do:** 
 - Make the annotation to Breakfast Dataset first, as described above; Write the annotations into a file so that it will be easily read by Python in the future.
 - Think about how to deal with "background" labels in the gtea dataset and this can be further discussed in the next meeting. 

## Additional Notes
Check the total available storage of the spartan account. 
