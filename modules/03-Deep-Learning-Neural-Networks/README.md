# Module 03 — Deep Learning & Neural Networks

## Learning Objectives

By the end of this module students will:

- Understand the structure of a neural network (neurons, layers, weights)
- Explain how deep learning differs from classical machine learning
- Identify key architectures: CNNs, RNNs, Transformers
- Appreciate how deep learning powers modern AI (vision, speech, NLP)

---

## Topics Covered

### 1. From ML to Deep Learning

Classical ML algorithms (decision trees, linear regression, SVMs) require humans to manually select and engineer the features the model uses. Deep learning removes this step — given enough data, deep neural networks learn which features matter on their own. This is why deep learning dramatically outperforms classical ML on complex tasks like image recognition, speech transcription, and language understanding, where the relevant features are too subtle and numerous to hand-engineer.

### 2. Biological vs Artificial Neurons

The artificial neuron is loosely inspired by the biological neuron in the human brain. A biological neuron receives signals from other neurons, processes them, and fires if the combined input exceeds a threshold. An artificial neuron similarly receives numeric inputs, multiplies each by a **weight** (representing importance), sums them up, and applies an **activation function** to decide its output. The analogy is imperfect — artificial neural networks work very differently from biological brains — but it provides useful intuition.

### 3. Neural Network Architecture — Input, Hidden, Output Layers

A feedforward neural network has three types of layers:

**Input layer:** Receives the raw data. For image recognition, each pixel is one input neuron. For text, each token is encoded as a number.

**Hidden layers:** Intermediate layers that transform the input through weighted connections and activation functions. Each layer learns increasingly abstract representations of the data. Early layers detect simple features (edges in images, common word patterns in text); deeper layers detect complex combinations (faces, sentences, concepts).

**Output layer:** Produces the final prediction. For a binary classifier, this is a single neuron outputting a probability. For a 10-class image classifier, there are 10 output neurons — one per class.

"Deep" learning refers to networks with many hidden layers — modern LLMs have hundreds.

### 4. Activation Functions, Weights, and Backpropagation

**Weights** are the learnable parameters of the network — each connection between neurons has a weight that determines how much one neuron influences another.

**Activation functions** introduce non-linearity, allowing the network to learn complex patterns. Common functions: ReLU (Rectified Linear Unit), Sigmoid, Tanh.

**Backpropagation** is the training algorithm. After the network makes a prediction, the error is calculated (the "loss"). Backpropagation calculates how much each weight contributed to the error, and those weights are then adjusted slightly to reduce the error. This is repeated across millions of training examples until the model performs well.

### 5. Convolutional Neural Networks (CNNs) — Image Recognition

CNNs are specifically designed for grid-structured data like images. Instead of connecting every neuron to every pixel, CNNs use **convolutional filters** — small windows that slide across the image detecting local features (edges, corners, textures). Early layers detect simple features; deeper layers combine them into complex shapes and objects. CNNs are the foundation of modern image recognition, object detection, and medical imaging AI.

### 6. Recurrent Neural Networks (RNNs) — Sequential Data

RNNs are designed for **sequential data** — text, speech, time series — where the order of inputs matters. Unlike feedforward networks that process each input independently, RNNs maintain a **hidden state** that carries information from previous inputs. This allows the network to "remember" context. However, standard RNNs struggle with long sequences. LSTM (Long Short-Term Memory) networks solve this by adding gates that control what to remember and forget.

### 7. Transformers — The Architecture Behind LLMs

The Transformer architecture, introduced in the 2017 paper "Attention Is All You Need," has become the dominant architecture in AI. Unlike RNNs, Transformers process all tokens in a sequence **in parallel** and use an **attention mechanism** to determine which tokens are most relevant to each other. This makes them dramatically faster to train and better at capturing long-range dependencies in text. Every major LLM — GPT-4, Claude, Gemini, Llama — is built on the Transformer architecture.

### 8. GPU Computing and Why It Matters

Training deep neural networks requires performing billions of floating-point multiplications in parallel. GPUs (Graphics Processing Units) were designed for this — they have thousands of simple cores that can perform these calculations simultaneously. Training GPT-3 required thousands of GPUs running for weeks. This is why AI development is concentrated at organisations with access to large GPU clusters, and why GPU chip companies like NVIDIA have become central to the AI industry.

---

## Demonstrations

- Visualising a neural network with TensorFlow Playground — live training in the browser
- Image classification with a pre-trained CNN (Google Colab)
- Transformer attention visualisation

## Hands-on Activities

- Experiment with TensorFlow Playground to tune a neural network on a spiral dataset
- Run a pre-trained image classifier on Google Colab (upload your own image)
- Visualise what layers "see" in a CNN using feature maps

## Assignment

Create a one-page visual explainer (diagram + text) of how a Transformer model processes a sentence. See `../../assessments/assignments/README.md` for full brief.

## Additional Resources

- [TensorFlow Playground](https://playground.tensorflow.org/)
- [3Blue1Brown — Neural Networks series](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)
- [Fast.ai Deep Learning Course](https://course.fast.ai/)

---

*Previous: [Module 02 — Machine Learning Fundamentals](../02-Machine-Learning-Fundamentals/README.md)  |  Next: [Module 04 — Generative AI & LLMs](../04-Generative-AI-and-LLMs/README.md)*
