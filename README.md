# BasketBall Analytics

## Training

### Prepare dataset

Please put the dataset in folder ./data with the following structure folder:
```sh
basketballanalytics/data/
                    |->training/
                    |     |-> image_2/00****.jpg
                    |     L-> label_2/00****.txt
                    L->ImageSets/
                          L-> train.txt
  ```
You can extract sample.tar.gz for example experiment.

### Run/start training

```sh
basketballanalytics$ bash script/train.sh -gpu 0 (change 0 with -1 if using cpu)
```
Check the trained model in ./models/train

### Monitor the training process

Open a new terminal and open a given output link in your favorite browser

```sh
basketballanalytics$ tensorboard --logdir=./models/train
```
# squeezeDet_test
