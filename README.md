---

# Eurecat datathon: From 0 to Data Scientist

---

Implementation of the solutions for the 
[Eurecat challenge](https://github.com/Applied-Artificial-Intelligence-Eurecat/hackeps) 
during Hack EPS 2022 edition. On Applied AI, mainly DL for CV.

Below you can find the same information as in the _DevPost_ project, but before
a list of the different ``README.md`` for each mission is presented:
- <a href="https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/yellow/README.md">Yellow mission</a>
- <a href="https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/red/README.md">Red mission</a>
- <a href="https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/orange/README.md">Orange mission</a>
- <a href="https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/purple/README.md">Purple mission</a>
- <a href="https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/green/README.md">Green mission</a>
- <a href="https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/black/README.md">Black mission</a>

### Relevant links
Also I attach some links that may prove useful: 
- Local notebooks in the repo (I pushed them in this repo even though I developed them in Kaggle):
  - [Orange mission: local notebook](https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/orange/Eurecat%20-%20Orange.ipynb)
  - [Purple mission: local notebook](https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/purple/Eurecat%20-%20Purple.ipynb)
  - [Green mission: local notebook](https://github.com/gcastro-98/eurecat-datathon-applied-ai/blob/main/green/Eurecat%20-%20Green.ipynb)
- Kaggle notebooks where I developed the code (I needed GPU):
  - [Orange mission: Kaggle notebook](https://www.kaggle.com/code/gerardcastro/eurecat-orange)
  - [Purple mission: Kaggle notebook](https://www.kaggle.com/gcastro98dev/eurecat-purple)
  - [Green mission: Kaggle notebook](https://www.kaggle.com/gerardcastro/eurecat-green)


Finally, in this link you can find the serialization of (large pretrained) models both for the orange and purple
missions: [link](https://we.tl/t-PnON5LQ4d0)

## Inspiration
Most of the proposed challeges are DL tasks, for they require CV approaches. 
I was eager to understand how the implementations of several techniques 
(such as transformers or capsum) worked. 
That's why I took profit and I used this challenge to learn them

## What it does
- Solves most of the proposed missions by Eurecat
- Provides a summary of the proposed implementations

## How we built it
Using Python, specifically:
- Tensorflow, mainly through the Keras API
- Numpy and pandas
For the supervised learning part I built data pipelines,
which were also responsible for the data augmentation 
process. Then both pre-trained models (CNN such as 
- ``EfficientNet`` & transformers such as ``ViT16``) using transfer learning,
as well as CNN from scratch, were built, trained and used. 

## Challenges we ran into
- Finite computational power & time-consuming trainings
- I worked in parallel implementing the different solutions, and so need
more accounts for the Kaggle part
- Hard to serialize and to store pre-trained CNN and transformers

## Accomplishments that we're proud of
- Solve most of the challenges, having into account I could not join 
the hackaton before 4pm and I was alone

## What we learned
- How to perform transfer learning with Visual Transformers (ViT).
- How to explain DL models for CV task using Captum

## What's next for  From 0 to Data Scientist - Eurecat
There are many improvements to be made, mostly regarding the fine-tuning part.
Currently, the training process is so basic that just prevents over-fitting.
However, te following could be controled:
- Dropout tuning
- Different optimizers with different learning rates schedulers
- Mainly, changes to the backbone
- Finally, more explainability job (even though is not required)
in the sense it helps during the model training. For instance,
salency maps for the differents channels could have been constructed.
- Oversampling the images corresponding to under-represented classes
- Improve even more the data augmentation process
