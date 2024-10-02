---
layout: default
---

## Towards Diverse and Consistent Typography Generation

![Concept](https://raw.githubusercontent.com/CyberAgentAILab/tdc-typography-generation/projectpage/images/teaser.jpg)

Wataru Shimoda<sup>1</sup>, Daichi Haraguchi<sup>2</sup>, Seiichi Uchida<sup>2</sup>, Kota Yamaguchi<sup>1</sup>  
<sup>1</sup>CyberAgent.Inc, <sup>2</sup> Kyushu University  

### Abstruct
In this work, we consider the typography generation task that aims at producing diverse typographic styling for the given graphic document. We formulate typography generation as a fine-grained attribute generation for multiple text elements and build an autoregressive model to generate diverse typography that matches the input design context. We further propose a simple yet effective sampling approach that respects the consistency and distinction principle of typography so that generated examples share consistent typographic styling across text elements. Our empirical study shows that our model successfully generates diverse typographic designs while preserving a consistent typographic structure.


### Results
<img src = "https://raw.githubusercontent.com/CyberAgentAILab/tdc-typography-generation/projectpage/images/res.png" title = "res">

### Results with different diversity  
<img src = "https://raw.githubusercontent.com/CyberAgentAILab/tdc-typography-generation/projectpage/images/diverseexample.png" title = "cmp">

### Citation

```bibtex
@misc{shimoda_2024_tdctg,
    author    = {Shimoda, Wataru and Haraguchi, Daichi and Uchida, Seiichi and Yamaguchi, Kota},
    title     = {Towards Diverse and Consistent Typography Generation},
    publisher = {arXiv:2309.02099},
    year      = {2024},
}
```