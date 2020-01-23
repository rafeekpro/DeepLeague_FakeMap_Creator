# Image Generator for AI

From one image you can create a lot of images with random mask

Get from github
```
git clone 
```

Inside directory install virtual environemnt
```
python -v virtualenv venv
```

Activate 
```
source venv/bin/activate
```

Install all dependency
```
pip -r install requirements.txt
```

Create directory where you store your images
```
mkdir base_images
```

Create directory where you store masks
```
mkdir cover_images
```

## Run program

For run program we need 
- at least one image to convert eg.  
```
base_images/image1.png
````
- at least one mask
```
cover_images/mask1.png
```
- if we wnat YOLOv3 file we must label that image and puy result in 
```
base_images/image1.txt
```
Results will be stored in *output* direcotry

```
python generator.py -i base_images/image1.png -O image1 -n 100 -l base_images/image1.txt 
```
