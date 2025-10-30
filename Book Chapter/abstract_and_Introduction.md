# Abstract

Progressive steps were taken by deep learning models in a multitude of applications, such as hyperspectral image processing and natural language processing.  
The main source of interest in this study is the **Convolutional Neural Network (CNN)**, which is regarded as one of the most powerful methods for learning image representations and semantic features.

This research examines several deep learning architectures — including **ResNet50, DenseNet201, AlexNet, and VGG16** — to detect breast cancer from mammogram images.  
A dataset of **1312 ultrasound images** (both benign and malignant) was used to train and validate the models.

The models were evaluated based on their **accuracy, precision, recall, and F1-scores**, with the base CNN model (enhanced using **Keras Tuner** and **data augmentation**) achieving the **highest accuracy of 88%**, outperforming transfer learning approaches.  

By leveraging CNN-based architectures and augmentation techniques, the study demonstrates that deep learning can assist in **early and reliable detection of breast cancer**, reducing both false negatives and unnecessary medical interventions.


# Introduction

Breast cancer is a frequent disease with a high fatality rate, particularly among
women. As a result, the greatest strategy for combating this condition is early exam-
ination. For visualizing the breasts, a set of modalities are available, notably
mammography, tomosynthesis, molecular breast imaging, and magnetic resonance
imaging. Mammography is the most prevalent analytical procedure among them
because of its ubiquity and inexpensive cost. Mammography pathognomonic is
the most often used accurate technology for initial identification of carcinoma.
Deep learning, pertinently deep convolutional neural networks (CNNs), which
may be easily implemented with cutting-edge performance, plays an essential role
in improving outcomes in the domain of biomedical engineering. Many people still
utilize mammography as their primary approach. It examines the human breast with
low-dose X-rays. On mammography, malignant tumors and calcium accumulation
appear prominent. Mammography now serves as the global standard strategy to miti-
gate breast cancer mostly in the beginning phases, prior tumors become clinically
conspicuous.

Breast malignancies are broadly categorized into two types: benign and malig-
nant. Benign lesions are noninvasive (noncancerous), whereas malignant lesions
are pathogenic (cancerous). The infectious stage of a condition determines whether
it is benign or malignant. Tumors serve as the most predominant clinical criterion of
carcinomas, which are present as grayish to white in pixel luminosity readings on
mammograms. Throughout the breast region, breast lumps differ in intensity, disper-
sion, structure (pedunculated, anomalous, spherical, elliptical), and boundaries (spi-
culated, inadequately, constricted), enhancing the hazard of misinterpretation are
shown in Fig. 9.1.

Various levels, comprising pooling layers and convolutional and fully linked
layers, are characteristic of the CNN design for mammography [1]. The convolu-
tional layers utilize filtration to acquire distinctive features from mammography im-
ages, whereas the pooling layers down-sample the feature mappings to substantially
minimize computation and preserve merely the most significant traits. The
Computational Intelligence and Modelling Techniques for Disease Detection in Mammogram Images. 
completely linked layers incorporate the preceding layers’ characteristics and create
the ultimate categorization or detection decision. CNN is supervised on a tremen-
dous database of mammography pictures designated as carcinogenic or noncarcino-
genic in breast cancer diagnosis. The model begins to identify cancer-related
structures and characteristics in visuals. CNN is determined to assess abnormal sec-
tions in mammography pictures that require additional inspection in lesion
segmentation.

The goal of this research is to look at approaches to give a deep learning (DL)
method that can adequately distinguish malignant neoplasm so that premature med-
ications might indeed be prevented because of incorrect negatives and inefficient
treatments can be eliminated owing to wrongful convictions. A database of 1312 im-
ages comprises both sorts of photographs, that is, the labels benign and malignant
have been employed. The models VGG16, DenseNet201, AlexNet, and ResNet50
are used. Without any transfer learning, we attain the best accuracy for our basic
model [2]. Augmentation is a technique for rescaling data and reducing overfitting.
When evaluated on a widely used accessible dataset, the presented approach yields
good results. Pretrained techniques are also helpful in healthcare image processing,
as they execute exactly with a low loss rate. These methodologies are developed on
vast datasets of mammography pictures and can evolve to distinguish cancer-related
structures and attributes.

Numerous DL approaches, notably CNN, have subsequently achieved spectac-
ular outcomes in a variety of fields, involving malignancy prediction, skin carcinoma
analysis, and breast cancer screening. CNN is the most extensively utilized deep
learning approach, allowing for automatic mass categorization, pattern recognition,
and segmentation with minimal training datasets and no human interaction. CNNs
are built in a layer structure. Furthermore, Deep Learning algorithms have demon-
strated remarkable advancements in the medical arena, providing researchers confi-
dence that patients may now securely interface with an activated medical equipment
and participate in a significant role in enhancing patient healthcare. Owing to the
inherent constraints of traditional approaches, we demonstrate a method that utilizes
deep learning in this study, exhibiting the capabilities of CNNs to identify. Breast
microcalcifications are segmented to aid radiologists in mammography analysis.
Step by step procedure is shown in Fig. 9.2.
