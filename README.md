# dynamic_link_prediction_through_GDES

 <!-- Dependencies -->
Create a Conda virtual environment and install all the necessary packages

'''
conda create --name GDES python=3.9
conda activate GDES
'''

'''
conda install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch
pip install tqdm
pip install torch_geometric
pip install pandas
pip install scikit-learn
pip install modelscope
pip install pytorch_lightning
pip install transformers
'''

<!-- Datasets -->
We use `bert` and `qwen` for text feature extraction and address search embedding, which can be found in the `dataset`([Baidu Cloud link](https://pan.baidu.com/s/1PlFWuetez--3sqL6adDzvQ) extraction code **6666**). And we also utilize adjacency matrix information in `adjacency_matrix` folder

<!-- Usage -->
To reproduce the code, please focus on the `GDES.py` and `NHPE.py` files. We use the data from the `dataset` and `adjacency_matrix` folders. You only need to replace the specified paths in `NHPE.py` and `GDES.py` with your corresponding paths.

- `embedding_path_qwen`: the embedding of qwen
- `embedding_path_bert`: the embedding of bert
- `adj17_path`: the adjacency matrix in 2023-06-30
- `a15_path`: the adjacency matrix in 2022-06-30
- `industry_path`: the information of industry_chain
- `node_index`: the index of nodes
- `location_path_qwen`: the embedding of location
- `location_path_bert`: the embedding of location
- `edge_status_json`: counting of node pairs
