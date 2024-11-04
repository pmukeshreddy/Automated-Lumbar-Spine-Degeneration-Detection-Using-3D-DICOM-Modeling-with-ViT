This project, Automated Lumbar Spine Degeneration Detection Using 3D DICOM Modeling with ViT and EfficientNet, leverages advanced deep learning architectures to detect degenerative changes in the lumbar spine using medical imaging data. The approach combines Vision Transformers (ViT) and EfficientNet to analyze 3D DICOM images, offering an automated solution that aims to enhance diagnostic accuracy in medical imaging.

The Vision Transformer (ViT) component of the model is applied to handle the spatial complexity of lumbar spine images, which often contain intricate details that can be challenging for conventional models. ViT is known for its effectiveness in image classification tasks by breaking down images into patches and processing them in a manner similar to natural language processing, capturing long-range dependencies within an image. This characteristic makes it particularly suitable for analyzing high-resolution images like those in 3D DICOM format, where capturing subtle details across slices is essential.

In addition to the Vision Transformer, EfficientNet is used to further enhance the model's ability to classify degeneration levels accurately. EfficientNet's design, which optimizes the balance between depth, width, and resolution of the neural network, allows it to achieve high performance with minimal computational overhead. By combining EfficientNet with ViT, this model leverages the strengths of both architectures, achieving robust and efficient classification results for medical imaging data.

This repository includes all necessary components for data preprocessing, model training, and evaluation. The dataset is expected to consist of DICOM files organized in a structure that facilitates training on 3D volumetric data. Several preprocessing steps, including intensity rescaling and resizing, are performed to ensure that the model receives consistent and appropriately scaled input data. The project employs a 5-fold cross-validation setup to ensure robust performance across different subsets of the data, maximizing the generalizability of the model.

Overall, this project demonstrates the application of modern deep learning techniques for automated medical image analysis, focusing on a clinically significant problem: detecting lumbar spine degeneration. The model’s design emphasizes accuracy, computational efficiency, and the potential for real-world clinical implementation, ultimately aiming to assist radiologists in making faster and more accurate diagnoses.






