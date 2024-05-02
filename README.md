
## Usage

1. **Loading and Preprocessing Data**: The data is loaded from a CSV file and preprocessed. Time column is dropped, and the 'Amount' column is scaled using StandardScaler.

2. **Creating a Masked Dataset**: A geometric mask is applied to the training data to create a masked dataset.

3. **Building the Autoencoder Model**: An autoencoder model is built with a dense input layer, a hidden layer with ReLU activation, and a dense output layer with sigmoid activation.

4. **Building the Discriminator Model**: A discriminator model is built with two hidden layers with ReLU activation and a dense output layer with sigmoid activation.

5. **Training the Autoencoder**: The autoencoder model is trained using the masked dataset. Training is performed for a specified number of epochs and batch size.

6. **Training the Discriminator**: The discriminator model is trained using both real and fake data generated by the autoencoder. Training is performed for a specified number of epochs and batch size.

7. **Detecting Anomalies and Setting Thresholds**: Anomalies are detected using the trained autoencoder model. An MSE threshold is calculated based on the anomaly scores, and anomalies are identified based on this threshold.

## Contributing

Contributions are welcome! Please feel free to open a pull request for any improvements or new features.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
