
# Simple Knowledge Distillation using KANs on MNIST Handwritten Digits
This project implements the KAN architecture, which utilizes learnable activation functions on the edges of the network with parametrized spline functions, replacing traditional fixed activation functions and linear weights. This approach offers a promising alternative to Multi-Layer Perceptrons (MLPs), with potential applications in data fitting, Partial Differential Equations (PDEs) solving, and more.

Here I have used the KAN implementation to distill a deep teacher KAN with 3 layers:
```
teacher_model = KAN([28*28, 64, 10])
```

to a lighter student model with 2 layers:
```
student_model = KAN([28*28, 10])
```

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

## Results
The MNIST dataset is a very simple dataset which may cause a very negligible increase in accuracy from a non-distilled model to a distilled model.
```
Accuracy of the NOT distilled student model on the test set: 93.65%
Accuracy of the DISTILLED student model on the test set: 93.75%
Accuracy of the teacher model on the test set: 97.23%
```

## Support

For support, open an issue through the GitHub issue tracker.

## License

This software is released under the MIT License.
