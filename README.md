# CoLA: Convolutional Neural Network Model for Secure Low Overhead Logic Locking Assignment

CoLA stands as a convolutional neural network (CNN) model tailored to the task of logic locking assignment, with a specific emphasis on minimizing overhead. To establish an effective logic locking method that can offer robust security against a wide range of potential attacks while imposing minimal additional area overhead, a deep comprehension of the underlying circuit architecture is essential. In pursuit of this objective, this document begins by constructing a multi-label dataset through the execution of diverse attacks on benchmark circuits previously secured with established logic locking techniques, encompassing a variety of key sizes. This dataset captures the level of security and associated overhead for each benchmark.

Subsequently, we introduce and evaluate CoLA, a convolutional neural network model specifically designed to process this dataset. CoLA's training involves the analysis of extracted features from the benchmark circuits, allowing it to effectively map circuits to secure, low-overhead locking schemes. Notably, CoLA is empowered to discern features that extend beyond a mere structural perspective by considering various resynthesized versions of the same circuits.

To expedite the process of assigning locking schemes to new, unseen data, we employ a quantization technique designed to reduce the computational burden of feature extraction during classification. The results, based on an extensive dataset comprising over 10,000 instances, demonstrate consistently high accuracy in both the training and validation phases. These findings underscore the efficacy of our approach in achieving secure and efficient logic locking for circuits.

The folder ``Dataset'' contains 75 elements of the dataset needed to run the experiment. To extend the amount of the dataset, data extension methods are suggested which are available in Keras. 

# Citation
```
@INPROCEEDINGS{CoLA,
  author={Aghamohammadi, Yeganeh and Rezaei, Amin},
  booktitle={Proceedings of the Great Lakes Symposium on VLSI (GLSVLSI)}, 
  title={CoLA: Convolutional Neural Network Model for Secure Low Overhead Logic Locking Assignment}, 
  year={2023},
  volume={},
  number={},
  pages={339–344},
  doi={10.1145/3583781.3590219}
}
