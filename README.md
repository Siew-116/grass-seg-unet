# grass-seg-unet
## v1 
- follow same hyperparameter
- result: bad metrics around 0.1
  
## v2 
- class weight: sqrt weight (+pixel calcuation from train dataset)
- learning rate = 1e-4 (P1), 1e-5 (P2)
- loss function: weighted sparse categorical cross entropy
- augmentation: add tf.cond to horizontal flip and vertical flip
- result: model 2 have better metrics, but model 1 better visual for test predictions
