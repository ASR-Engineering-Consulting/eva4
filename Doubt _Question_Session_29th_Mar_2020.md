### Doubt Clear Session (29th March 2020) - Hosted by "The School of AI"

> Good Morning


> For GradCAM, we have to access layers. And I saw two ways of doing it. Using hook and other way. Can you please elaborate on hook?


> a quick refresher on how grad cam works ? using that diagram from grad cam paper


> Data augmentation - does it add images or just does transformation on images?


> need some clarity around normalizarion values, (0.5,0.5,0.5) why these, on web there are some other values for cifar10.does it have something to do about oytorch


> IF same number of parameters are there then the deeper layer will get trained faster as compared to a shallow network ... Sir can this be elaborated


> Do we have any plan to use OpenCv


> I understand that model is copied batch size times and each copy takes one image,calculates weights and corrects them using backprop.


> hi sir does it make sense to use LR scheduling with adaptive LR algorithms? or should we stick to just ReduceLROnPlateau?


> need some clarification about actual effect of L1 and L2


> In LR Finder, what range of LR should we send the algorithm to test and for how many iterations? I tried various ranges and compared the loss in each of them. I got the least loss in:


> start: 1e-10, end: 100, iterations: 740 ==> lr: 0.008, but I think that a loss 0.008 would be extremely less as a starting point. Can you please shed some light on this?


> I understand L1 and L2 norm but m confused under which circumstances to L1 and when to use L2


> Does increasing Batch size improves test accuracy ?


> Why don't we use dropout with cutout, as you taught


> why using Receptive field higher than image size give better performance


> Is there a separate session on Backpropagation also ?


> Hi, how to calculate parameters in depthwise and grouped convolution. also pls explain grouped convolution.


> Can you explain pixel shuffle algorithm again?


> I felt that reducing LR to 10% of original value is too steep.. Is it standard to reduce to 10%? (in most of the codes I see it is 10%)


> In AdaptiveAvgPool2d if the input is 7x7x512 and we pass it to nn.AdaptiveAvgPool2d(3), the output becomes 3x3x512. In this case, how is the mean calculated so that the output shape becomes 3x3?


> LRFinder, StepLR ,1 Cycle LR policy -> Are all these methods meant to find the LR i.e. LR that gives us least loss ?


> Also is following understanding correct -> We will find best LR by running against validation data for 1 epoch (multiple iterations) , take this LR and use it for training remaining epochs ?


> is it okay to use lr finder to find 4-5 lrs, they would be fluctuating, and taking the mean of those lrs and use it


> Watch fastai explanation after sir's explanation on pixel shuffle you will be able to get a good grasp of the concept


> SGD has other parameter, weight decay & dampening. Where these should be used?


> What's gradient accumulation? Is it used when we have large number of classes(hence large batch size)?


> In GradCam, the outcome from calculations is yielding similar values, resulting unicolor in heat map. What may be computed incorrectly.


> Any reason why Dilated Convolutions were not added in ResNet architecture? Is it because we have multiple RFs already in the last layers which is enough to give good accuracy


> In the inception model we have auxiliary losses so that we can infuse new gradients when the gradients die out in between ..


> Is this thing used even after the invention of batch normalisation which helps in preserving the gradients ?


> from LRfinder, should we take the LR which has the steepest decrease (even if loss range is high) compared to the LR in a crevice (in the loss vs LR graph) which has lower loss.


> how to target individual class accuracy, given the fact that particular class may have less images compared to other classes that's why accuracy is dropping for that class


> I am training resnet18 and saving the model parameters, optimizer parameters and last epoch as a checkpoint. After that i am loading the all the saved parameters as a checkpoint for retraining.......


> First of all, Will that be considered a valid training for a model?


> I was getting the problem of overfitting when i use Albumentation , can you explain the cause of it?


> Secondly, why the train accuracy bumps up in the first re-train epoch and then settles down to a value nearby what it was in the last epooch of the last check out?


> Sir suppose my network works best with n*n images and I scale all my images to n*n how much wrong is this and why ?


> if we have no memory constraint, which one to choose fully connected or average pool? which one give better accuracy


> Is it possible to combine mobile net and unet


> in CIFAR10, even though model test accuracy is around 92+% but for few classes accuracy is around 80%, any techniques to improve accuracy for non-preforming classes


> in Keras there is a way to penalize or increase the loss for specific classes. In pytorch not very though


> In practices, we just define train and testing loader. How do we get validation loader? What is the best practices of creating validation set?


> Is there a difference in how you use optimizations like batch normalization , especially between training mode and inference mode?


> You said that in LR finder, we should take the LR with the least loss. In an experiment, I got least loss with LR 0.008, isn't it too small as a initial LR?


> Sir data leakage means that nothing should be seen from the validation set but when we normalize data we use mean of entire data which has validation data also so isn't it leading to data leakage ?


> In one of the blog i read that Taylor series is used to approximate the loss function based on weight parameters. Is it True ?


> Should we also use GAP for pre trained network


> do we have session on transferlearning, improving network while doing transfer learning. suppose I want to add bn or dropout in inception, how to do that when I am simply using learnt network


> Why is SGD not used for small dataset


> Came across Captum library from PyTorch, they have IntegratedGradients, Saliency, DeepLift and NoiseTunnel? Will it give different insights as compared to GradCAM?


> There is this paper on using layer wise optimization with very large batches (up to 32k) would you recommend it in any of our assignments.


> is masking is based on gradcam concept only. how is masking applied


> masking done*


> We could resize the CIFAR dataset to 64x64 or 128x128 to get higher resolution at last layer. Will it impact the accuracy of model?


> can u give brief chronology from resnet, inception, exception... till date, I want to know type of architecture names for further reading


> In a paper I read depthwise separable convolution are usually implemented without non-linearity(ReLU). How does it work then? Is there any specific case for this?


> Also where all can we use depthwise separable convolution other than the case that if we have to reduce number of parameters.


> Follo up question "We could resize the CIFAR dataset to 64x64 or 128x128 to get higher resolution at last layer." As it will impact the accuracy, and we still need to do it for doing gradCAM?


> Please provide a brief idea about why GPU works faster for specific calculations. I mean it has a lot more cores than CPU. If that is the reason, a cpu with more cores would also work same.


> Is it preferable to use One-Cycle LR over Cyclic LR (when using SGD + momentum).


> Sir can you please repeat about Stochastic Resnet training and its benefits if any ?


> can you explain again, what gets computed on gpu and cpu in the cycle of DNN, and when do we transfer to and fro


> for images that are square but actual information is rectangular with unwanted pixels(black) on left and right sides(like those in eip4 final assignment ),what is the best way to handle?


> At what stage of Deep Learning do we use the Quantization? Is it during training or validation?


> when you say data augmentation is done on cpu,how come it is so fast considering large number of images?Not much difference in time is seen with or without augmentation


> sir you told that mixup will need to predict both cat and dog so what kind of loss function would be there?


> Your thoughts on why Resnet architectures perform better in PyTorch and inception architectures perform better in Keras


> Where are we in terms progress of Phase1, any specific feedback looking into our assignment. Where we should spend more time on? I see implementation/coding has bigger role.


> Any reference to get upto speed on the coding in PyTorch?


> Any suggestions on list of papers to be read, in the topics covered so far?


> do we have libraries to convert from tensorfliw to pytorch and viceversa


> BBye!
