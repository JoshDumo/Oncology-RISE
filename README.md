# Oncology-RISE
# **Colorectal histopathology**
## Classification of textures

Histopathologists study and diagnose diseases in tissues by examining the tissues under a microscope [1]. This technique is particularly useful in diagnosing cancer, where tissue obtained from suspicious lumps can be analyzed and classified if cancerous. The preparation of tissues for imaging is an involved process, but it can be summarized broadly into three steps: fixation, staining, and mounting [2,3]. Fixation is done to keep the tissue as life-like as possible, by preserving it in chemical agents like fomaldehyde. Staining enhances the visualization of organelles and membranes. The tissue is then mounted on glass slides for support so they can be imaged.  Once the preparation is done the tissue can be imaged under a microscope and digitized.

Here we develop a system that uses AI/ML based image classification to classify tissue from digital images from colorectal histopathology. Colorectal images are obtained from ref [4] which is provided on Tensorflow Datasets catalog. The images are used to train a CNN network using Tensorflow. The resulting model is used to classify the images into one of 8 classes: 'Tumor', 'Stroma', 'Complex', 'Lympho', 'Debris','Mucosa', 'Adipose', and 'Empty'.

In addition, we use Randomized Image Sampling for Explanation (RISE) to provide a measure of explainability for the model [5]. This is important for these 'mission critical' applications. We note also that, especially for medical applications, the effective approach is what is now being called "AI + X", where AI is not a replacement of expertise, but rather an augmentation.
