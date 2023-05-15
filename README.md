# VCSum: A Versatile Chinese Meeting Summarization Dataset

Han Wu, Mingjie Zhan, Haochen Tan, Zhaohui Hou, Ding Liang and Linqi Song.

Abstract: Compared to news and chat summarization, the development of meeting summarization is 
hugely decelerated by the limited data. To this end, we introduce a versatile Chinese meeting 
summarization dataset, dubbed VCSum, consisting of 239 real-life meetings, with a total 
duration of over 230 hours. We claim our dataset is ***versatile*** because we provide the 
annotations of topic segmentation, headlines, segmentation summaries, overall meeting summaries, 
and salient sentences for each meeting transcript. As such, the dataset can adapt to various 
summarization tasks or methods, including segmentation-based summarization, multi-granularity 
summarization and retrieval-then-generate summarization. Our analysis confirms the effectiveness 
and robustness  of VCSum. We also provide a set of benchmark models regarding different 
downstream summarization tasks on VCSum to facilitate further research.

**We are preparing the release of the data. We will release it once the reviewing process of SenseTime is 
finished.**

## Data Samples

We provide five pieces of data samples from our dataset for your convenience. There are two files, 
i.e., `data_samples.txt` and `highlight_samples.txt`.

The `data_samples.txt` contains the annotations of topic segmentation, headlines, segmentation summary and overall 
meeting summary. The keys in the `dict` are:

- `id`: the unique identifiers of the meeting transcript.
- `eos_index`: the utterance positions of topic segmentation.
- `speaker`: the speaker identifier.
- `context`: the meeting transcript.
- `summary`: the overall meeting summary.
- `discussions`: the list of segmentation summaries.
- `headlines`: the list of headlines.

The `highlight_samples.txt` file provides the annotations of highlight sentences.

- `id`: the unique identifiers of the meeting transcript.
- `highlights`: the 0/1 list of context words. 1 stands for the highlighted word.
