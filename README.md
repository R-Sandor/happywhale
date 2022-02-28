# Happywhale
CS795/895 Practical Machine Learning (Spring, 2022) Project I


# Tasks To-do
- ~~Download images directly from Kaggle, there are too many images for github to hold (40gb between train/test) https://www.kaggle.com/c/happy-whale-and-dolphin/data~~
- ~~Break down the species into two categories i.e. whales and dolphins.~~
  - The training csv includes species feature. 
    - Be mindful that some species have whale in the title but are dolphins, e.g. killer whales.
      - Do you mean killer whales actually are dolphins? I thought it only some typos like "kiler whales" but still considered as whales.
- Research different ways to process images.
  - Consider turning the images into monochrome as the professor has discussed. 
    - This is a good point if we want to use some classifier algos like logistics regression, so we don't need many channel features but only one channel would be sufficient 
    to find fin contour. This could be applied before we do some edge detection operations.
  - Figure out how to do bounding boxes? Will we need to do object recognition? 
    - This can be done by using **edge detection operations** on images. But this means we assume only the shape of dorsal fins is the most vital feature for classification. 
    Is this ture?
  - YOLO for dorsal fin object dection. 
    - Will need to create a label for dorsal fins if this approach is taken.
    - promising methods but involves much labelling stuff, could borrow the idea of bounding boxes.
- Create the IEE report template to fill out the findings. 
  - found in link: https://www.overleaf.com/articles/prospects-for-a-next-generation-deep-space-network/fwdmqzvtrgwb

- **Pipeline of our idea: RGB images --> monochrome image --> edge detections --> proposed bounding boxes into our classifier algo (logistic regression) --> final classification result**


