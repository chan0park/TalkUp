# TalkUp Dataset
This repository contains a collection of data and resources related to the "TalkUp: A Novel Dataset Paving the Way for Understanding Empowering Language" paper. 

## Dataset Description
The TalkUp dataset is designed to provide insights into empowering language usage in various contexts. It includes data collected through AMT, utilizing a carefully crafted annotation user interface (UI). TalkUp can be used to train language models that capture empowering and disempowering language. More broadly, as it is rich with the ambiguities and diverse interpretations of real-world language, TalkUp provides an avenue to explore implication, presuppositions, and how social context influences the meaning of language. 

## Data File
The actual data is stored in the CSV file named `talk-up-2000.csv`. This file contains 2000 instances of collected data along with various attributes that can be utilized for analysis and research purposes. The dataset comprises several columns, each providing specific information related to the instances collected. Here is a brief explanation of each column:

1. **subreddit**: The subreddit where the post and response pair occurred.
2. **poster**: The gender of the person who made the post.
3. **post**: The text of the post.
4. **response**: The text of a comment left on the post.
5. **model_generated**: Indicates whether this sample was discovered by a ML model or randomly sampled.
6. **empower**: Aggregated label indicating whether this example is empowering, neutral, or disempowering.
7. **reasons**: Reasons of empowerment marked by annotators. Only the ones that at least 2 out of 3 annotators agreed on are kept.
8. **stance**: Aggregated label indicating whether the annotators believed the responder agrees or disagrees with the poster.
9. **ambiguity**: Marked as 'yes' if any one of the three annotators thought "this post can be interpreted as either empowering or disempowering depending on what the poster meant," or if all three annotators disagreed on the label (i.e., one empowering, one disempowering, one neutral). Otherwise, marked as 'no'.
10. **empower_all**: All three annotations from the three annotators (not aggregated).

Please refer to the paper for a comprehensive overview of the dataset, including the specific details and meanings of each column.

## Annotation UI
We have included the annotation UI HTML file used during the data collection process. You can find it in the repository under the name `amt-annotation-UI.html`. This file served as the interface through which the AMT workers annotated the dataset. The annotation file also include the task instruction we provided to AMT annotators. Feel free to adapt this file for your own annotation.

## Paper Reference
If you use this dataset in your research or refer to it, please cite the following paper:
> **TalkUp: A Novel Dataset Paving the Way for Understanding Empowering Language**<br>
> Authors: [Insert authors' names]<br>
> Conference/Journal: [Insert conference/journal name]

## Contact Information
For any questions related to the TalkUp dataset, please contact `chanyoun@cs.cmu.edu`. We welcome feedback and suggestions to improve the data set.

## Usage and Licensing
The TalkUp dataset is made available under the MIT License. Please review the license file in this repository for detailed information regarding the terms of use.
