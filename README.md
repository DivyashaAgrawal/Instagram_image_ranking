# Instagram_image_ranking
Amazon ACMS


# Image ranking project(Instagram)
.

We have scrapped the images using Instagra-scraper(Forked from  rarcega/instagram-scraper)
 

Cmd:
python triplet_sampler.py --input_directory <<path to the directory>> --output_directory <<path to the directory>> --num_pos_images <<Number of positive images you want>> --num_neg_images <<Number of negative images you want>>
```

```
Example: python triplet_sampler.py --input_directory similarity_images --output_directory triplet_folder --num_pos_images 10 --num_neg_images 50
```
## How to get the similarity distance between two images?

The "deepranking_get_distance.py" calculates the similarity distance between the two images and prints it out. The script takes 3 inputs:
1) The deepranking model file (h5 file)
2) Image 1
3) Image 2

```
Format: python deepranking_get_distance.py --model <<path to the model>> --image1 <<path to image 1>> --image2 <<path to image 2>>
```

```
Example: python deepranking_get_distance.py --model ./deepranking.h5 --image1 ./image1.jpg --image2 ./image2.jpg
```


