# Housing-Price-Prediction


The idea of this project was to create a predictor on the California housing dataset. The data pertains to the houses found in a given California district and some summary stats about them based on the 1990 census data.

<img width="316" height="276" alt="3" src="https://github.com/user-attachments/assets/c61ee378-37d5-48a4-bf00-85aa9698222d" />
<img width="392" height="262" alt="4" src="https://github.com/user-attachments/assets/cc0623db-27c6-4f8e-823b-91e769178ba6" />
<img width="1177" height="862" alt="1" src="https://github.com/user-attachments/assets/c6018ad7-f4ff-4d1d-930e-de32cf001956" />
<img width="330" height="285" alt="5" src="https://github.com/user-attachments/assets/f9d16162-38a9-4886-b016-88fc16c59576" />
<img width="1166" height="862" alt="2" src="https://github.com/user-attachments/assets/6d65bdac-181b-4954-9e37-7f6c9fff2640" />



## The data

The data is comprised of 8 attributes

* MedInc median income in block

* HouseAge median house age in block

* AveRooms average number of rooms

* AveBedrms average number of bedrooms

* Population block population

* AveOccup average house occupancy

* Latitude house block latitude

* Longitude house block longitude

as well as the target, the housing price

## Training

`train.py` runs the training for three different models: NN, linear regression, and random forest on the scikit-learn California housing dataset:

```bash
python3 train.py
```

Training output example:

```bash
...

Train Epoch: 150 [0/18576 (0%)] Loss: 0.130984
100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 37/37 [00:00<00:00, 143.57it/s]
5
100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 102.93it/s]
        NN
r2 score: 0.8232532827300671
MAE score: 0.2833885734455647
        Linear regressor
r2 score: 0.6098033978087847
MAE score: 0.4635741867691994
        Random forest
r2 score: 0.8138137169848451
MAE score: 0.2837869675577879
...
```


## Conclusion

The neural network trained on the standardized signals gave the best model with an R2 score of 82.4. The models trained on the first two principal components gave a poor result, even if they accounted for ~96% of the data variance.

## 👤 Author

**HOSEN ARAFAT**  

Software Engineer, China 

GitHub: https://github.com/arafathosense

Researcher: Artificial Intelligence, Machine Learning, Deep Learning, Computer Vision, Image Processing
