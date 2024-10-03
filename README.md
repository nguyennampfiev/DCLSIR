# Fine tuning of Destruction and Construction Learning for Fine-grained Image Recognition for Stamp Retrieval

## Training

Run `train.py` to train DCL.

For training CHAM from scratch

```shell
python train.py --data CHAM --epoch 360 --backbone resnet50 \
                    --tb 16 --tnw 16 --vb 512 --vnw 16 \
                    --lr 0.0008 --lr_step 60 \
                    --cls_lr_ratio 10 --start_epoch 0 \
                    --detail training_descibe --size 192 \
                    --crop 192 --cls_mul --swap_num 5 5
```
For test see notebook file