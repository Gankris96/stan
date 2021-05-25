# To run the code - 
## 1. Python version 3.8 or above
## 2. Install all required dependencies  
        pip install -r requirements.txt
## 3. Run the preprocessing step in Data_Processing folder
### a. Set the url to the appropriate Capture file and run the python notebook. 
### b. Set the output file name

## 4. Run the STAN model to generate data.
### a. Again, set the right file name in https://github.com/Gankris96/stan/blob/master/examples/ugr16_data_maker.py#L24 
### b. Similarly set the validation data path.
### c. Run prepare_rawdata if you are running on a new raw csv - https://github.com/Gankris96/stan/blob/master/examples/ugr16_data_maker.py#L149 
### d. You can run runner_train https://github.com/Gankris96/stan/blob/master/examples/ugr16_data_maker.py#L162
### e. And runner_sample https://github.com/Gankris96/stan/blob/master/examples/ugr16_data_maker.py#L162 to generate samples for each ip addr.

## 5. Set the args as required, for example you can change the epochs. 
## 6. To run the code with your settings - 
        CUDA_VISIBLE_DEVICES=0 python ugr16_data_maker.py


