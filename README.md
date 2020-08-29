# Image-Colorizer
Coloring Black and White Images

We were recently watching a classic and historic Bollywood Movie which was originally in black and white, now colorized. 
This made us eager to try something like this using deep learning. So, we decided to start with colouring black and white images. 
Today, colorization is done by hand in Photoshop. A picture can take up to one month to colorize. It requires extensive research. 
A face alone needs up to 20 layers of pink, green and blue shades to get it just right. So, we thought of trying this using neural networks. 
First attempt was to train a model on input image and get results based on that. This gave us very great result as the model was trained on one image only. 
Second, we used the inception resnet v2 — a network trained on 1.2M images. This way model will try to generalize color schema on unknown images.
Starting with few images and a smaller number of epochs didn’t yield any good results. 
We gradually increased training data and epochs and ended up with images having more of a red shade. 
Major issue was hardware i.e. if we had more GPU power, we can train around 10k images 10K images with 21 epochs will take about 11 hours on a Tesla K80 GPU.
