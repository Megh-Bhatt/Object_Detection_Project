## Object Detection Project
The journey begins with transforming the 28x28 pixel grayscale images into flat vectors, preparing them for the network's processing power. Then, the first layer, aptly named "Flatten," performs this crucial task.
Next, the data journeys through two hidden layers, each containing 128 neurons. These neurons act like tiny detectives, diligently analyzing the information, identifying subtle nuances that differentiate a sneaker from a sandal. To introduce non-linearity and complexity into the network's decision-making, a special activation function called "relu" is employed in these layers.
Finally, the data reaches the output layer, where 10 neurons stand ready, each representing a different clothing category. Armed with the knowledge gleaned from the previous layers, these neurons strive to predict the correct label for each image. Softmax, a clever mathematical trick, ensures that the outputs add up to 1, interpreting them as probabilities for each category.<p>

But how does the network learn? Imagine a teacher patiently guiding its student. Here, the role of the teacher is played by the training process. By showing the network thousands of labeled images, it gradually adjusts its internal connections, learning to differentiate between a T-shirt's smooth curves and a shoe's intricate laces. The "Adam" optimizer acts as the fine-tuning tool, meticulously adjusting the connections to minimize errors and improve the network's accuracy.
After 10 rounds of learning (known as epochs), the network is put to the test on a set of unseen images. This test reveals its true potential – how well it can generalize its knowledge to new examples. The "test_acc" value proudly displayed is a testament to its learning ability.

#### Results
![Screenshot 2024-02-18 192745](https://github.com/Megh-Bhatt/Object_Detection_Project/assets/98394685/b2fe4b9a-549c-42e9-8307-1d4333067c33)

#### Libraries and their Roles
1. TensorFlow: The core library for building and training the neural network model. It provides the building blocks for defining layers, loss functions, optimizers, and performing training and evaluation.
2. NumPy: Used for numerical computations and data manipulation. It efficiently handles the conversion of 2D images to 1D vectors as input for the network and performs array operations for calculations.
3. Matplotlib: Used for data visualization. It creates the plots showcasing sample images, their predicted labels, and probability distributions, providing visual insights into the model's predictions.
#### How to use on your local device

 - Download the repository
 - make a new folder extract the files in it
 - Install necessary packages using pip install -r requirements.txt.
 - After finally downloading the requirements you can run the code and train and experiment with the model
