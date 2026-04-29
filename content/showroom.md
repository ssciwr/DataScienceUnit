# Showroom

## Machine learning for Causal Sets in Quantum Gravity

TODO: add images

TODO: write model card and data card

TODO: select one model that works well on the 20k data

**Project partners**: Quantum gravity group, Prof. Dr. Astrid Eichhorn

### Topic
The causal set approach is a promising candidate for a theory of quantum gravity, but so far has been limited by the
diverse set of possible causal sets, which makes picking out suitable models for space time difficult.
Machine learning techniques can help with this problem by learning to classify causal sets according to their structure automatically,
thus allowing us to work with this large set of possibilities more effectively.

### Objective
This project pioneers the application of machine learning techniques to the causal set approach to quantum gravity.
Using an [existing software for the generation of causal sets developed in Prof. Eichhorn's group](https://codeberg.org/cyclopentane/CausalSets.jl), we apply deep learning techniques to classify causal sets according to their viability as models for space time.

### Project outcome
Together with our project partners from the Quantum gravity group, we extended the causal set generation algorithms to diversify the possible training data. Using this software, we then trained a graph neural network to classify causal sets according to whether they have a manifold-like structure and thus are viable models for space time. We found that the graph neural network was able to learn to classify causal sets with high accuracy, thus demonstrating the potential of machine learning techniques for this problem.
We used the Julia programming language for data generation, and employed the `pytorch-geometric` library for the implementation of the graph neural network.

We created two software packages, one for the data generation and machine learning library, and one for the experiment setup and training of the graph neural network. Both packages are available on GitHub, and the data and models are available on HugginFace.

### Enabling new research
Knowledge tranfer was an important part of the project, and we integrated our project partners early into the development process to ensure that they are able to use and extend the developed software and apply machine learning in their research.
Future work includes, among others, the application of generative models. A publication is currently in preparation.


You can find the software repositories and data here:
<div class="grid cards" markdown>

-   :material-xml:{ .lg .middle } __QuantumGrav__

    ---
    The main repository contains the code for data generation and the machine learning model code.

    [:octicons-arrow-right-24: Find it on GitHub](https://github.com/ssciwr/QuantumGrav)

    ---


-   :material-rocket-launch:{ .lg .middle } __QuantumGrav-usage__

    ---
    The experiment repository contains the code for the experiment setup and training of the graph neural network.

    [:octicons-arrow-right-24: Find it on GitHub](https://github.com/ssciwr/QuantumGrav-usage)


-   :material-data-matrix:{ .lg .middle } __Data__

    ---
    The training data contains a large set of causal sets of different types for training the machine learning model.

    [:octicons-arrow-right-24: Download the training data here](https://huggingface.co/datasets/MaHaWo/causal_sets_20k)

-   :material-robot:{ .lg .middle } __Model__

    ---
    The trained model can be used to classify new causal sets according to their viability as models for space time.

    [:octicons-arrow-right-24: Check out the model on huggingface](https://huggingface.co/MaHaWo/CS_classifier)


</div>
