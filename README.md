## Project thesis

This project thesis was made as part of the integrated five-year Master’s degree programme in Electronics Systems Design and Innovation at NTNU, Trondheim. The project thesis is a part of the course TFE4580 Electronic Systems Design and Innovation, Specialization Project, fall 2025, and is made in collaboration with Nordic Semiconductor.  

The project explores Artificial Neural Network (ANN) to Spiking Neural Network (SNN) conversion for Low-Power Embedded AI targeting MLPerf™ Tiny Deep Learning Benchmarks using ANNarchy. 

The jupyter notebooks contain the experiments done in relation to the project. The general structure and content of the files are similar for all experiments. First, the used dataset is imported, and some preprocessing steps are done. Then the model architecture is defined, trained and saved as a .keras file. Then the conversion module from ANNarchy is initialized and the trained ANN model is loaded and converted. Then the converted SNN makes predictions on the test set and the accuracy of both the ANN and the SNN is reported. 

The following table gives an overview of what the different files contain. 

<table>
  <thead>
    <tr>
      <th>File Name</th>
      <th>Dataset</th>
      <th>Model/Description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>ANNarchy.ipynb</td><td>MNIST</td><td>CNN from ANNarchy</td></tr>
    <tr><td>ANNarchyCIFAR_v1.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy</td></tr>
    <tr><td>ANNarchyCIFAR_v2.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy with batchnorm</td></tr>
    <tr><td>ANNarchyCIFAR_v3.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy with dropout</td></tr>
    <tr><td>ANNarchyCIFAR_v4.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy w/o batchnorm 3 blocks</td></tr>
    <tr><td>ANNarchyCIFAR_v5.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy w/o batchnorm 3 blocks explicit activation layer, epochs = 20</td></tr>
    <tr><td>ANNarchyCIFAR_v6.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy w/o batchnorm 3 blocks explicit activation layer, epochs=100</td></tr>
    <tr><td>ANNarchyCIFAR_v7.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy, epochs = 100</td></tr>
    <tr><td>ANNarchyCIFAR_v8.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy, epochs = 100, duration_per_sample = 400</td></tr>
    <tr><td>ANNarchyCIFAR_v9.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy, epochs = 100, duration_per_sample = 1000</td></tr>
    <tr><td>ANNarchyCIFAR_v12.ipynb</td><td>CIFAR10</td><td>VGG with dropout, epochs=100</td></tr>
    <tr><td>ANNarchyCIFAR_v13.ipynb</td><td>CIFAR10</td><td>VGG with dropout and data augmentation, epochs=100</td></tr>
    <tr><td>ANNarchyCIFAR_v14.ipynb</td><td>CIFAR10</td><td>VGG with increasing dropout and batchNorm, epochs=100</td></tr>
    <tr><td>ANNarchyCIFAR_v15.ipynb</td><td>CIFAR10</td><td>VGG-16</td></tr>
    <tr><td>ANNarchyCIFAR_v16.ipynb</td><td>CIFAR10</td><td>VGG-16, removed last two maxpool layers</td></tr>
    <tr><td>ANNarchyCIFAR_v17.ipynb</td><td>CIFAR10</td><td>VGG with dropout, epochs=100, same as B20 with add two conv layers</td></tr>
    <tr><td>ANNarchyCIFAR_v19.ipynb</td><td>CIFAR10</td><td>VGG with dropout, epochs=100, duration per sample = 200</td></tr>
    <tr><td>ANNarchyCIFAR_v20.ipynb</td><td>CIFAR10</td><td>VGG with dropout, epochs=100, duration per sample = 400</td></tr>
    <tr><td>ANNarchyCIFAR_v21.ipynb</td><td>CIFAR10</td><td>VGG with dropout, epochs=100, duration per sample = 1000</td></tr>
    <tr><td>ANNarchyCIFAR_v22.ipynb</td><td>CIFAR10</td><td>VGG with dropout, epochs=100, duration per sample = 2000</td></tr>
    <tr><td>ANNarchyCIFAR_v23.ipynb</td><td>CIFAR10</td><td>VGG with dropout, epochs=100, duration per sample = 300</td></tr>
    <tr><td>ANNarchyCIFAR_v24.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy, epochs = 100, duration_per_sample = 300</td></tr>
    <tr><td>ANNarchyCIFAR_v25.ipynb</td><td>CIFAR10</td><td>CNN from ANNarchy, epochs = 100, duration_per_sample = 2000</td></tr>
    <tr><td>ANNarchyMNIST_2.ipynb</td><td>MNIST</td><td>CNN from ANNarchy with batchnorm</td></tr>
    <tr><td>ANNarchyMNIST_v3.ipynb</td><td>MNIST</td><td>CNN from ANNarchy with dropout</td></tr>
    <tr><td>ANNarchyMNIST_v4.ipynb</td><td>MNIST</td><td>CNN from ANNarchy w/o batchnorm 3 blocks</td></tr>
    <tr><td>ANNarchyMNIST_v5.ipynb</td><td>MNIST</td><td>CNN from ANNarchy w/o batchnorm 3 blocks explicit activation layer, epochs =20</td></tr>
    <tr><td>ANNarchyMNIST_v6.ipynb</td><td>MNIST</td><td>CNN from ANNarchy w/o batchnorm 3 blocks explicit activation layer, epochs=100</td></tr>
    <tr><td>ANNarchy_CIFAR10_ResNet.ipynb</td><td>CIFAR10</td><td>ResNet</td></tr>
    <tr><td>ANNarchy_CIFAR10_VGG.ipynb</td><td>CIFAR10</td><td>VGG</td></tr>
    <tr><td>CIFAR.png</td><td></td><td>Picture of samples from CIFAR-10 dataset</td></tr>
    <tr><td>MNIST.png</td><td></td><td>Picture of samples from MNIST dataset</td></tr>
    <tr><td>cnn_annarchy_ann_accuracy.png</td><td></td><td>Plot of accuracy and loss of ANN traned in ANNarchyCIFAR_v7.ipynb</td></tr>
    <tr><td>datasets.ipynb</td><td></td><td>Script for rploting samples from datasets</td></tr>
    <tr><td>vgglike_ann_accuracy.png</td><td></td><td>Plot of accuracy and loss of ANN traned in ANNarchyCIFAR_v21.ipynb</td></tr>
  </tbody>
</table>

