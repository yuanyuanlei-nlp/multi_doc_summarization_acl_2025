# Read Me


**Paper:** Multi-document Summarization through Multi-document Event Relation Graph Reasoning in LLMs: a case study in Framing Bias Mitigation<br/>
**Accepted:** The Proceedings of the 2025 Annual Meeting of the Association for Computational Linguistics (ACL 2025)<br/>
**Authors:** Yuanyuan Lei, Ruihong Huang<br/>
**Paper Link:** https://aclanthology.org/2025.acl-long.1291/

<br/>

## Dataset Description

* **NeuS dataset:** a multi-document summarization dataset (https://github.com/HLTCHKUST/framing-bias-metric/tree/main/data). The articles with different political stances that discuss the same event are grouped together as a cluster.


<br/>

## Model Generated Summaries

We release the generated summaries from different models:

* **generated_summary_NeuS:** the generated summaries on NeuS dataset
  * _test_data folder:_ the test set, including the input articles and human written reference for each cluster of articles, the generated summaries from each model are listed in the order of test_0, test_1, ..., test_306 in each txt file below
  * _llama_baseline.txt:_ the generated summaries from Llama-2 baseline model
  * _llama_event_relation_graph.txt:_ the generated summaries from Llama-2 + event relation graph model
  * _led_baseline.txt:_ the generated summaries from Longformer-Encoder-Decoder (LED) baseline model
  * _led_event_relation_graph.txt:_ the generated summaries from LED + event relation graph model
  * _lexrank.txt:_ the generated summaries from LexRank baseline
  * _bart_large_cnn.txt:_ the generated summaries from BART-CNN baseline
  * _bart_large_multi.txt:_ the generated summaries from BART-Multi baseline
  * _pegasus_cnn.txt:_ the generated summaries from Pegasus-CNN baseline
  * _pegasus_multi.txt:_ the generated summaries from Pegasus-Multi baseline
  * _neus.txt:_ the generated summaries from NeuS baseline model (https://aclanthology.org/2022.naacl-main.228/)



<br/>


## Citation

If you are going to cite this paper, please use the form:


Yuanyuan Lei and Ruihong Huang. 2025. Multi-document Summarization through Multi-document Event Relation Graph Reasoning in LLMs: a case study in Framing Bias Mitigation. In Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers), pages 26603–26619, Vienna, Austria. Association for Computational Linguistics.


```bibtex
@inproceedings{lei-huang-2025-multi,
    title = "Multi-document Summarization through Multi-document Event Relation Graph Reasoning in {LLM}s: a case study in Framing Bias Mitigation",
    author = "Lei, Yuanyuan  and
      Huang, Ruihong",
    editor = "Che, Wanxiang  and
      Nabende, Joyce  and
      Shutova, Ekaterina  and
      Pilehvar, Mohammad Taher",
    booktitle = "Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2025",
    address = "Vienna, Austria",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.acl-long.1291/",
    pages = "26603--26619",
    ISBN = "979-8-89176-251-0",
    abstract = "Media outlets are becoming more partisan and polarized nowadays. Most previous work focused on detecting media bias. In this paper, we aim to mitigate media bias by generating a neutralized summary given multiple articles presenting different ideological views. Motivated by the critical role of events and event relations in media bias detection, we propose to increase awareness of bias in LLMs via multi-document events reasoning and use a multi-document event relation graph to guide the summarization process. This graph contains rich event information useful to reveal bias: four common types of in-doc event relations to reflect content framing bias, cross-doc event coreference relation to reveal content selection bias, and event-level moral opinions to highlight opinionated framing bias. We further develop two strategies to incorporate the multi-document event relation graph for neutralized summarization. Firstly, we convert a graph into natural language descriptions and feed the textualized graph into LLMs as a part of a hard text prompt. Secondly, we encode the graph with graph attention network and insert the graph embedding into LLMs as a soft prompt. Both automatic evaluation and human evaluation confirm that our approach effectively mitigates both lexical and informational media bias, and meanwhile improves content preservation."
}
```











