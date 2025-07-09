# Fineweb-zhtw

Most of this code is based on [Datatrove](https://github.com/huggingface/datatrove) and is licensed under the Apache 2.0 License.

## Installation
Clone repo with submodules
```bash
git clone --recurse-submodules https://github.com/mtkresearch/fineweb-zhtw.git
```

Install requirements
```bash
pip install -r requirements.txt
```

## To Run

prepare data for pipeline demonstration (download 2 WARC files)
⚠️ **Warning:** This download utilizes data from Common Crawl. Please review the [Common Crawl Terms of Use](https://commoncrawl.org/terms-of-use) before proceeding.

```bash
bash scripts/get_data_example.sh
```

run cleaning
```bash
bash scripts/map_warc_to_zhtw_text.sh
```
Results would be under `data/parsed/{DUMP}/5_zhtwplus/output`

If you like our work, please cite
```
@misc{lin2024finewebzhtwscalablecurationtraditional,
      title={FineWeb-zhtw: Scalable Curation of Traditional Chinese Text Data from the Web}, 
      author={Cheng-Wei Lin and Wan-Hsuan Hsieh and Kai-Xin Guan and Chan-Jan Hsu and Chia-Chen Kuo and Chuan-Lin Lai and Chung-Wei Chung and Ming-Jen Wang and Da-Shan Shiu},
      year={2024},
      eprint={2411.16387},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2411.16387}, 
}
@misc{penedo2024datatrove,
  author = {Penedo, Guilherme and Kydlíček, Hynek and Cappelli, Alessandro and Sasko, Mario and Wolf, Thomas},
  title = {DataTrove: large scale data processing},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  url = {https://github.com/huggingface/datatrove}
}
```

