## Paper: Can GPTs Evaluate Graphic Design Based on Design Principles?
Daichi Haraguchi<sup>1</sup>, Naoto Inoue<sup>1</sup>, Wataru Shimoda<sup>1</sup>, Hayato Mitani<sup>2</sup>, Seiichi Uchida<sup>2</sup>, Kota Yamaguchi<sup>1</sup>  
<sup>1</sup>CyberAgent.Inc, <sup>2</sup> Kyushu University  
Accepted to SIGGRAPH Asia (Technical Communications Track).
[[Project-page](https://cyberagentailab.github.io/Graphic-design-evaluation/)]

## Introduction
This repository contains the data for "Can GPTs Evaluate Graphic Design Based on Design Principles?".

<img src = "https://github.com/CyberAgentAILab/Graphic-design-evaluation/blob/projectpage/docs/images/teaser.jpg" title = "teaser" >

## Data
<pre>
./GPT_eval_data
├── gpt_eval
      ├── gpt_abs_alignment.csv
      ...
      └── gpt_comp_whitespace.csv
├── human_eval_data
      ├── human_abs_alignment.csv
      ...
      └── human_comp_whitespace.csv
└── images.zip
</pre>
Each CSV file includes the evaluation results.
File names consist of "[eval method]_[eval type]\_[design principle].csv."  
Note:  
"eval. method" is "gpt" or "human."  
"eval. type" is "abs" (absolute evaluation) or "comp" (comparative (relative) evaluation).  
"design principle" is "alignment," "overlap," or "whitespace."  

Example:  
"gpt_abs_alignment.csv" is the absolute evaluation result by GPT for alignment. 

"images.zip" includes images.  
The structure in the "images.zip" is below.
<pre>
images
├── lefttop_large
      ├── [image_ID].png
      ...
      └── [image_ID].png
...
└── org
      ├── [image_ID].png
      ...
      └── [image_ID].png
</pre>

Note:  
The directory name consists of "[perturbation element]_[perturbation size]"  
"Org" includes original images without perturbation.  
Each image name is an image ID that is written in the CSV files.  



## The structure of each CSV file
CSV for absolute evaluation
| id | perturbation | 0 | 1 | 2 | 3 | 4 | avg |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| image ID | perturbation size | score | score | score | score | score |average score|

CSV for relative evaluation
| id | comparative | better_design_0 | better_design_1 | better_design_2 | better_design_3 | better_design_4 | voting_res |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| image ID | perturbation size of comparison image | voting result | voting result| voting result | voting result | voting result | aggregation of voting results|


## Visualization
We provides a notebook for showing results.  
- `scatter_plot.ipynb` shows the scatter plot between human evaluation and GPT evaluation.  

## Reference
```bibtex
@misc{
coming soon
}
```

## Contact
This repository is maintained by Daichi Haraguchi.  
E-mail: haraguchi_daichi_xa[at]cyberagent.co.jp
