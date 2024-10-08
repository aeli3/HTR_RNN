# Handwritten Text Recognition with RNN and CNN Backbone

This repository contains code for recognizing handwritten text using a combination of a Convolutional Neural Network (CNN) and a Recurrent Neural Network (RNN). The CNN serves as a feature extractor, while the RNN processes the extracted features for sequence recognition.

## Key Features

- **CNN Backbone**: Extracts visual features from the input image (handwritten text).
- **RNN Layer**: Processes the features and predicts character sequences.
- **CTC Loss**: Connectionist Temporal Classification (CTC) is used to align predictions with the input text.

## Requirements

To run the code, you need the following libraries:

- Python 3.x
- PyTorch (depending on your implementation)
- Pillow
- Matplotlib


## Model Architecture

1. **CNN Backbone**: A series of convolutional layers are used to extract features from the input image. These layers help capture spatial information from the handwritten text.
   
2. **RNN (LSTM/GRU)**: The RNN (either LSTM or GRU) processes the sequence of feature vectors from the CNN. This helps capture the temporal dependencies between different characters.

3. **CTC Layer**: The output from the RNN is passed through a fully connected layer followed by a CTC loss function. This helps map the predicted sequences to the target text.


## Results

The model can effectively recognize handwritten text, including both individual characters and sequences of words. Generalizes less well to deviating writing styles.

## Contributions

Feel free to submit pull requests for improvements or fixes. 

## License

This project is licensed under the MIT License.

---

### Contact

For any issues or questions, feel free to open an issue on the repository.

