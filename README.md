Ongoing project...

What's new:
- Added style-based learning using a mapping network and AdaIN, similar to StyleGAN1.
- Added conditional training by modifying the SLE layers.
- Switched to PyTorch DDP.

Before training make sure your image folders are as following format:

```
images_folder
├── cat_images  (class1)
├── dog_images  (class2)
├── bird_images (class3)
└── ...         (class n)
```

Then your images directory will be: "D:\YourDir\images_folder"

How to train:

```batch
python train.py --dir D:\YourDir\YourFolder --inf
```
You can enable conditional training anytime by adding "--cond".
