# LION

This is the official PyTorch implementation of our IJCAI 2023 paper:

> [**LION: Label Disambiguation for Semi-supervised Facial Expression Recognition with Progressive Negative Learning**](https://www.ijcai.org/proceedings/2023/0078.pdf)      

## Requirements

We test the codes in the following environments, other versions may also be compatible:

- Python==3.6.9
- PyTorch==1.3.0
- Torchvision==0.4.1

## Dataset setup

Please download the dataset from [RAF-DB](http://www.whdeng.cn/raf/model1.html) website and change the root to your path. The splits of different-class labeled data are listed below. For example, for the case of 100 labels, the labeled training set consists of 10 faces annotated with fear and 15 faces annotated with other expressions. More details could be found in the supplementary material, which is available at CVF website. 

<table align="center">
    <tr>
        <th> </th>
        <th align="center" colspan=1>100 labels</th>
        <th align="center" colspan=1>400 labels</th>
        <th align="center" colspan=1>1000 labels</th>
        <th align="center" colspan=1>2000 labels</th>
        <th align="center" colspan=1>4000 labels</th>
    </tr>
    <tr>
        <td align="left">Fear</td>
        <td align="center">10</td>
        <td align="center">40</td>
        <td align="center">100</td>
        <td align="center">200</td>
        <td align="center">250</td>
    </tr>
    <tr>
        <td align="left">Others</td>
        <td align="center">15</td>
        <td align="center">60</td>
        <td align="center">150</td>
        <td align="center">300</td>
        <td align="center">625</td>
    </tr>
</table>

## Getting Started

To train on RAF-DB:

```bash
python main.py
```

## Citation

If you find our work useful in your research, please consider citing:

    @inproceedings{du2023lion,
      title={LION: Label Disambiguation for Semi-supervised Facial Expression Recognition with Progressive Negative Learning},
      author={Du, Zhongjing and Jiang, Xu and Peng, Wang and Zhou, Qizheng and Wu, Xi and Zhou, Jiliu and Wang, Yan},
      booktitle={Proceedings of the Thirty-Second International Joint Conference on Artificial Intelligence Main Track},
      month={July},
      year={2023},
      pages={699-707}
    }

