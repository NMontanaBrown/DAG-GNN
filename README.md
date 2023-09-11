# DAG-GNN

Adapting DAG-GNN to the synthetic data experiments in upcoming paper.

## Installing

```bash
conda create -n daggnn python=3.7
conda activate daggnn
conda install pytorch=1.10
pip install matplotlib pandas numpy seaborn
```

## Running synthetic experiments
To run the baseline experiments for DAG-GNN on the synthetic experiments, run the following commands from the `src` directory

### Sangiovese Grapes Dataset

```bash
python train.py --data_type real --data_filename grapes/grapes_data_clean.csv --data_sample_size 100000 --data_variable_size 14 
```

### Arctic Sea Ice Dataset

```bash
python train.py --data_type real --data_filename arctic/arctic_data_clean.csv --data_sample_size 468 --data_variable_size 12
```

### Alzheimer's Disease Dataset

```bash
python train.py --data_type real --data_filename alzheimers/alzheimers_data_clean.csv --data_sample_size 1000 --data_variable_size 9
```

## Getting results 

Run the provided jupyter notebook to get the results for the synthetic experiments at `data/dag_gnn.ipynb`.

## Cite

If you make use of this code in your own work, please cite the original paper:

```
@inproceedings{yu2019dag,
  title={DAG-GNN: DAG Structure Learning with Graph Neural Networks},
  author={Yue Yu, Jie Chen, Tian Gao, and Mo Yu},
  booktitle={Proceedings of the 36th International Conference on Machine Learning},
  year={2019}
}
```



