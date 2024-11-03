This project aims to develop a deep learning pipeline for classifying lumbar spine degeneration using 3D DICOM image reconstructions. The model leverages Vision Transformers (ViT) and a custom implementation of EfficientNet for 3D volumetric data to achieve accurate classification, as part of the RSNA 2024 Lumbar Spine Degenerative Classification Challenge. By integrating advanced neural architectures, the project addresses the complex task of automatically identifying degenerative changes in lumbar spine images.

The dataset consists of DICOM images provided by RSNA, organized by subject and series. Each subject folder contains one or more DICOM series, from which 3D volumes are constructed with an image shape of (128, 128, 128, 3). To standardize the input, we preprocess the images using torchio for intensity scaling and resizing. This step is essential for ensuring consistent input dimensions across the model and enhancing model performance on 3D medical imaging data.

This project incorporates two main deep learning architectures. First, Vision Transformers (ViT) are adapted to handle 3D inputs for processing volumetric data effectively. Second, a custom implementation of EfficientNet is manually tailored for 3D DICOM data, providing flexibility without relying on pre-built libraries. These models classify the 3D spine images, assessing different degeneration levels in the lumbar spine.

Initial experiments were conducted with a learning rate of 0.001 and a batch size of 4. The dataset image size of (128, 128, 128, 3) ensures that the 3D context is maintained, which is essential for capturing the degenerative patterns in the spine. Model performance is evaluated using recall (ADR) and precision. Our best results to date include a recall of 0.9959 and a precision of 0.6090, indicating a strong balance in the model’s ability to correctly identify positive cases.







