
# Simple Knowledge Distillation using KANs on MNIST Handwritten Digits
This project implements the KAN architecture, which utilizes learnable activation functions on the edges of the network with parametrized spline functions, replacing traditional fixed activation functions and linear weights. This approach offers a promising alternative to Multi-Layer Perceptrons (MLPs), with potential applications in data fitting, Partial Differential Equations (PDEs) solving, and more.

The KAN code is referenced from the [efficient_kan](https://github.com/Blealtan/efficient-kan) repository.

Get started with KAN-Distillation by following these steps:

1. **Clone the Repository:**
    ```
    git clone https://github.com/pranavgupta2603/KAN-Distillation
    ```
2. **Enter the directory**
    ```
    cd KAN-Distillation
    ```
2. **Install Dependencies:**
    ```
    pip install -r requirements.txt
    ```

## Documentation

- `distill.ipynb`: Contains the code to train the student model
- `mnist.py`: An extension to the code from [efficient_kan](https://github.com/Blealtan/efficient-kan) to train a non-distilled model
- `requirements.txt`: Contains all the necessary Python packages.

## Support

For support, open an issue through the GitHub issue tracker.

## License

This software is released under the MIT License.
