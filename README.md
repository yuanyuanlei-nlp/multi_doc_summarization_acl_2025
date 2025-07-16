# Read Me


**Paper:** Multi-document Summarization through Multi-document Event Relation Graph Reasoning in LLMs: a case study in Framing Bias Mitigation<br/>
**Accepted:** The Proceedings of the 2025 Annual Meeting of the Association for Computational Linguistics (ACL 2025)<br/>
**Authors:** Yuanyuan Lei, Ruihong Huang<br/>
**Paper Link:** https://arxiv.org/abs/2506.12978/

<br/>

## Dataset Description

* **NeuS dataset:** a multi-document summarization dataset (https://github.com/HLTCHKUST/framing-bias-metric/tree/main/data). The articles with different political stances that discuss the same event are grouped together as a cluster.


<br/>

## Model Generated Summaries

We release the generated summaries from different models:

* **generated_summary_NeuS:** the generated summaries on NeuS dataset
  * _test_data:_ the test set, the model generated summaries are listed in the order of test_0, test_1, ..., test_306
  * _llama_baseline:_ the generated summaries from Llama-2 baseline model
  * _llama_event_relation_graph:_ the generated summaries from Llama-2 + event relation graph model
  * _led_baseline:_ the generated summaries from Longformer-Encoder-Decoder (LED) baseline model
  * _led_event_relation_graph:_ the generated summaries from LED + event relation graph model
  * _lexrank:_ the generated summaries from LexRank model
  * _bart_large_cnn:_ the generated summaries from BART-CNN baseline
  * _bart_large_multi:_ the generated summaries from BART-Multi baseline
  * _pegasus_cnn:_ the generated summaries from Pegasus-CNN baseline
  * _pegasus_multi:_ the generated summaries from Pegasus-Multi baseline
  * _neus:_ the generated summaries from NeuS baseline model (https://aclanthology.org/2022.naacl-main.228/)


<br/>


## Citation

If you are going to cite this paper, please use the form:


```bibtex
@misc{lei2025multidocumentsummarizationmultidocumentevent,
      title={Multi-document Summarization through Multi-document Event Relation Graph Reasoning in LLMs: a case study in Framing Bias Mitigation}, 
      author={Yuanyuan Lei and Ruihong Huang},
      year={2025},
      eprint={2506.12978},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2506.12978}, 
}
```











