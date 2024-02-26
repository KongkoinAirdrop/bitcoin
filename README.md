BitcoinForecast
Predict bitcoin value for the next 9minutes, with Recurrental Neural Network GRU.
Requirements:
- python3
- keras 2
- numpy
- MatploitLib

Data
You can download data through the grabber.py

Instructions
Clone the repo:
git clone https://github.com/PiSimo/BitcoinForecast.git

Training on new data:
python3 network.py -train dataset_path -iterations number_of_training_iterations
To finetune the new model with an old one just add -finetune base_model_path to the line above.
At the end of the training you will have an updated model.h5 with the new weights and you will see a plot with the test results.

Running:
python3 network.py -run dataset_path -model model_path
The dataset is also required when you run, to perform normalization.
To visualize a plot with the real and predicted results enter Crtl-C and type no ,the program will create chart.png with the results.
