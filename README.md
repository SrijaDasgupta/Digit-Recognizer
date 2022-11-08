# Digit-Recognizer
Steps:
Read and preprocess the data
Define the model architecture
Define a callback function
Compile and Fit the model
Subclassing:
Custom Loss Function
Any callable with the signature loss_fn(y_true, y_pred) that returns an array of losses can be passed to compile() as a loss. Note that sample weighting is automatically supported for any such loss
Custom Layer
A layer is a callable object that takes as input one or more tensors and that outputs one or more tensors.
It involves computation, defined in the call() method, and a state (weight variables).
init(): Defines custom layer attributes
build(self, input_shape): This method can be used to create weights that depend on the shape(s) of the input(s)
call performs the logic of applying the layer to the inputs
Training a Model Using Subclassing
