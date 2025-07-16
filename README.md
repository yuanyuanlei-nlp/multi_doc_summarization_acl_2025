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
  * _test_data folder:_ the test set, including the input articles and human written references, the generated summaries from the below models are listed in the order of test_0, test_1, ..., test_306 in each txt file
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











