## This project was a kind of observation to see how better the transformer learn with and without stripping some of the information.

### data-format
* $ text -> interview transcript + seperator +  class1 + seperator + class2 and so on till 5 classes $
* completion tab has ClassName and END token concatenated at the end of the line.

**As a result the accuracy was much larger when the last labels were provided**

The data consists of the transcripts of the interviewer and the task is to identify the class of the tech stack the question is associated with.

> There are more than 150 classes and more than 2 lakh samples in the prompt.

- Model used distilbert-base-uncased-finetuned-sst-2-english

## Wandb Analysis Report
<!-- display images -->
<img src="InterviewClassification\charts\Section-2-Panel-0-3x8ff61ib.png" width="100%">
<img src="InterviewClassification\charts\Section-2-Panel-1-fnurli7dq.png" width="100%">
<img src="InterviewClassification\charts\Section-2-Panel-2-bqt23i8lw.png" width="100%">
<img src="InterviewClassification\charts\Section-2-Panel-3-ji3bwgkg8.png" width="100%">