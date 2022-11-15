# Bachelor's Thesis
Hosting a pdf version of my bachelor's thesis which involved generating videos that are in sync with a given audio segment. This involved a novel architecture trained on top of the latent space of a pretrained StyleGAN (FFHQ). The details are in the pdf of the thesis and a set of slides that I presented during my viva.

This framework is presented below.


![architecture](https://github.com/rsn870/Bachelor-s-Thesis/blob/main/images/thesis_arch.png)


Given an initial latent an LSTM model is used to predict the set of residuals corresponding to motion for each frame. We use a Facenet based Identity loss, an Audio Visual Sync Loss and a Novel Landmark Regression Loss to ensure that the new faces have the same identity and the right kind of motions.Some of our results on HD youtube videos that do not belong to our dataset are shown below 

![results](https://github.com/rsn870/Bachelor-s-Thesis/blob/main/images/lipsync_results.png)
