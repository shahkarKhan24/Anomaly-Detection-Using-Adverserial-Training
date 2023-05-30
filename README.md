# Anomaly-Detection-Using-Different Approaches in ImBalance Dataset

<h3> Baseline Technique<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</h3>
<p>The first method that we tried was using an autoencoder, Autoencoder is an unsupervised learning technique for neural networks that learns efficient data encoding by training the network to ignore signal noise. It simply consist of a simple encoder decoder network that when given an input image tries to reconstruct out the same image with minimum reconstruction loss.
 <div>
<img src="https://github.com/shahkarKhan24/Anomaly-Detection-Using-Adverserial-Training/blob/main/Images/auto%20mode.jpg?raw=true" width="700" alt="Baseline Architecture Figure"/>
</div>
 
</p>



<h3> SOTA Technique<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</h3>
<p> We tried the method that was described in the sota paper[1]. Which is also a Generative Adversarial Network (GAN) based architecture consist of a generator and two separate discriminators. Generator model is just like a simple U-net or an autoencoder and discriminator is a decoder like network.We try to minimize the reconstruction loss for normal data and maximize the reconstruction loss for Anomaly data, also a couple of different loss functions were introduced
 
 <div>
<img src="https://github.com/shahkarKhan24/Anomaly-Detection-Using-Adverserial-Training/blob/main/Images/SOTA.jpg?raw=true" width="700" alt="SOTA Architecture Figure"/>
</div>
</p>


<h3> Additional Non-Sota Technique <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</h3>
<p>The next method we tried was using GAN model which consist of simple generator and discriminator architecture. The generator's job is to create realistic-looking data, such as images, while the discriminator's role is to distinguish between real and fake data. The discriminator basically takes this generated sample and tries to determine if it's real or fake. The generator aims to generate samples that the discriminator cannot distinguish as fake, while the discriminator tries to become better at identifying fake samples. This back-and-forth training continues until the generator becomes skilled at producing realistic data that can fool the discriminator into thinking it's real.
 
<div>
<img src="https://github.com/shahkarKhan24/Anomaly-Detection-Using-Adverserial-Training/blob/main/Images/non_sota%20additional.jpg?raw=true" width="700" alt="Baseline Architecture Figure"/>
</div>
</p>





