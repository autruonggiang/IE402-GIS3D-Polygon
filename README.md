# Nghiên cứu về học biểu diễn đa năng cho hình học đa giác - IE402 Project

## **SOURCE CODE & RELATED CONTENT**  
- **GitHub Repository (Original Research Paper):**  
   🔗 [GitHub - polygon_encoder](https://github.com/gengchenmai/polygon_encoder)  

- **Model Training & Evaluation:**  
   🔗 [Colab - Model Training](https://colab.research.google.com/drive/1lTanYey5ZxqTCpBBdljNicaBrRVLjukw?usp=sharing)  

- **Prediction Demo:**  
   🔗 [Colab - Spatial Relation Prediction](https://colab.research.google.com/drive/1j9fGgpyP7h1zjPXYtubU2kLxvBwt8esd?usp=sharing)  

- **Project Presentation Slides:**  
   🎤 [Canva - GIS3D Presentation](https://www.canva.com/design/DAGZ7VVZdps/rjEIxWjiSedOkJWqkj8PfQ/edit)  

- **Demo on Streamlit:**  
   🔗 [Streamlit - GIS3D Demo](https://drive.google.com/file/d/1LVCVglIr1SnxvLbCCbzM4_GEEOswx-sZ/view?usp=sharing)  

## Related Link
1. [Springr Paper](https://link.springer.com/article/10.1007/s10707-022-00481-2)
2. [Arxiv Paper](https://arxiv.org/abs/2209.15458)

## Model Overview
<p align="center">
  <img src="image/model.png" alt="model" width="1000" />
</p>

## Dependencies
Required packages are summarized in `requirements.txt` and others.

## Data
Download the required dbtopo datasets from [here](https://www.dropbox.com/scl/fo/ubokquibjibxqb71lduto/h?rlkey=gnex7g3gx51g06gmd1v1um9u1&dl=0) and put them in `./data_proprocessing/dbtopo/output/` folder. The folder has two datasets:
1) DBSR-46K: the `pgon_triples_geom_300_norm_df.pkl`file, a GeoDataFrame contain the DBSR-46K spatial relation prediction dataset created from DBpedia and OpenStreetMap. Each row indicates a triple from DBpedia and its subject and object are presented as a simple polygon with 300 vertices.
2) DBSR-cplx46K: the `pgon_triples_geom_300_norm_df_complex.pkl` file, a  GeoDataFrame contain the spatial relation prediction dataset. The only difference is each row's subject and object are presented as a complex polygon with 300 vertices.



## Train and Evaluation
The main code are located in `polygoncode` folder

1) `1_pgon_dbtopo.sh` do suprevised training on both DBSR-46K and DBSR-cplx46K datasets.  



### Reference
If you find our work useful in your research please consider citing [our GeoInformatica 2023 paper](https://link.springer.com/article/10.1007/s10707-022-00481-2).  
```
@article{mai2023towards,
  title={Towards general-purpose representation learning of polygonal geometries},
  author={Mai, Gengchen and Jiang, Chiyu and Sun, Weiwei and Zhu, Rui and Xuan, Yao and Cai, Ling and Janowicz, Krzysztof and Ermon, Stefano and Lao, Ni},
  journal={GeoInformatica},
  volume={27},
  number={2},
  pages={289--340},
  year={2023},
  publisher={Springer}
}
```


Please go to [Dr. Gengchen Mai's Homepage](https://gengchenmai.github.io/) for more information about Spatially Explicit Machine Learning and Artificial Intelligence.
