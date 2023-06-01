# Poem Autocomplete Colab Notebook

This Colab Notebook provides a poem autocomplete feature. It suggests completions for a given input sequence of words. The model used in this notebook is trained on a custom dataset.

## Dataset

The dataset used for training the autocomplete model is stored in a file called `data.txt`. Each line in the file represents a poem. The dataset is tokenized and processed before training.

## Model Architecture

The autocomplete model is built using PyTorch. It consists of an embedding layer, an LSTM layer, and a linear layer. The model is trained to predict the next word in a sequence given a window of previous words.

## Usage

To use this Colab Notebook, follow these steps:

1. Import the required libraries by running the first code cell.

2. Import and optimize the dataset by running the second code cell. Make sure you have a file named `data.txt` in the same directory.

3. Preprocess the data by running the third code cell.

4. Define the model architecture by running the fourth code cell.

5. Train the model by running the fifth code cell. Training may take some time depending on the dataset size and training parameters.

6. Run the model by executing the last code cell. Adjust the settings in the form to specify the maximum length of the autocompletion, the seed value for the beam search, and the input sequence for which you want suggestions. The model will generate autocompletions using beam search and display the suggested completions.

## Examples

(length = 1; seed = 124) ` dreams come ` -> ` dreams come and `

(length = 3; seed = 1917) ` realm ` -> ` realm strides, lyrical springs `

(length = 7; seed = 2364) ` two souls ` -> ` two souls guarding gather, kindness roaring becomes sun passion's `

Feel free to experiment with different settings and input sequences to generate diverse poem suggestions.

## Contributing

Contributions to this project are welcome! If you have ideas for improvements or want to add new features, please create a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
