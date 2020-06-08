# image_captioning
Caption generation is a challenging artificial intelligence problem where a textual description
must be generated for a given photograph. It requires both methods from computer vision to
understand the content of the image and a language model from the field of natural language
processing to turn the understanding of the image into words in the right order. 

## Dataset
I used the Flickr8k dataset.
You can download dataset [here](http://academictorrents.com/details/9dea07ba660a722ae1008c4c8afdd303b6f6e53b)
Please notice that you download [utorrent](https://www.utorrent.com/desktop/) and install before downloading Flick8k.\
This dataset contains 8000 images each with 5 captions (as we have already seen in the Introduction section that an image can have multiple captions, all being relevant simultaneously).
These images are bifurcated as follows:\
	1. Training Set — 6000 images\
	2. Dev Set — 1000 images\
	3. Test Set — 1000 images

## Prepare photo data
I used a pre-trained model to interpret content of the photos. There are many model to choose from. In this project, I chose InceptionV3 model.

## Prepare text data
In order to  reduce the size of the vocabulary of words, the text data must be cleaned:\
	1. Convert all words to lowercase.\
	2. Remove all punctuation.\
	3. Remove all words that are one character or less in length (e.g. ‘a’).\
	4. Remove all words with numbers in them.
 
