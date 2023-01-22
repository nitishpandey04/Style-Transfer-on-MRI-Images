# Style-Transfer-on-MRI-Images

### Idea:
There are various types of MRI that have the ability to capture different types of abnormalities. However, one type of MRI may not be sufficient in capturing a particular type of abnormality. In this case, having another type of MRI may enhance the accuracy of a diagnosis, thus leading to better treatment of the patient.

However, gaining access to different imaging techniques is difficult and expensive. Also, doctors often prescribe one type of MRI at once, but what if we could create another type of MRI from the one that we already have? Moreover, without investing the same amount of time and money?

### Understanding:
Let’s understand the T1 and T2 type MRIs in concrete terms. There are some component types such as Water, Fat, Muscle and Tumors which establish contrast relationship between MRIs. Moreover some of the elements have different contrast level whereas Bone component in MRIs gets highlighted in the same way in both the MRIs. Hence we can see that it’s a partial contrast but not complete contrast. 

![T1 vs T2 table](https://github.com/nitishpandey04/Style-Transfer-on-MRI-Images/blob/master/t1_vs_t2_table.png)

As this is not a complete list of components that are highlighted in the MRIs, to learn more about T1 and T2 images, you may visit [here](https://www.radiologymasterclass.co.uk/tutorials/mri/t1_and_t2_images).

### Solution:
With the help of deep learning, we can use style transfer to generate artificial MRI images of different contrast levels from existing MRI scans. This will help to provide a better diagnosis with the help of an additional image.

In this project, we have used CycleGAN to translate the style of one MRI image to another, which will help in a better understanding of the scanned image. Using GANs we have created T2 weighted images from T1 weighted MRI image and vice-versa.

#### Tech Stack:
python, tensorflow, keras, numpy, pandas, matplotlib, skimage

#### Dataset
- The dataset is divided into two classes Tr1 and Tr2
- Tr1 contains 43 images and Tr2 contains 46 images
- You can access the dataset [here](https://huggingface.co/datasets/nitishpandey04/MRI-Unpaired-T1-and-T2-Images/blob/main/MRI_Dataset-20230122T105937Z-001.zip)
