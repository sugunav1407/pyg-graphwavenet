# GraphWavenet
PyG implementation of [Graph WaveNet for Deep Spatial-Temporal Graph Modeling](https://arxiv.org/pdf/1906.00121.pdf). The model takes a list of node embeddings across several time steps and predicts the output embeddings for the specified number of upcoming time steps.

We have tested the code on the METR-LA dataset, which is also used by the example. The results are comparable to the paper's baseline:
  ┌────────────────────┬──────┬──────┬────────┐
  │ Model              │ MAE  │ RMSE │ MAPE   │
  ├────────────────────┼──────┼──────┼────────┤
  │ Paper baseline     │ 3.53 │ 7.37 │ 10.01% │
  │ Our implementation │ 3.18 │ 6.34 │  8.87% │
  └────────────────────┴──────┴──────┴────────┘

The main model is implemented in the file graphwavenet.py
  
#Instructions
Run main.py. 
Note: Before running this file, run the following command to generate the dataset
python generate_data.py


  
