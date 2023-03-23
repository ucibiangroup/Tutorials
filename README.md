# Tutorials
Tutorials for new group members in Bian Lab
Please click star in the right corner.

## This repository has three training set, your learning sequence is:  
1. MnistConvnet.ipynb(the dataset has been integrated in Keras)  
2. Convnets_with_small_datasets(cat_vs_dog).ipynb(the dataset is in the server /storage/data/tutorials/dogs-vs-cats)  
3. Convnets_with_pretrained_datasets(cat_vs_dog).ipynb(the dataset is in the server /storage/data/tutorials/dogs-vs-cats)  


## Connect to Lab Server
1. Download Cisco VPN here: https://www.oit.uci.edu/services/security/vpn/  
2. Contact admin of the server to get an account on the server such as you@muon-neutrino.ps.uci.edu, and an initial password.  
3. Connect to the server with your initial password:  
```$ssh you@muon-neutrino.ps.uci.edu```  
4. Change your initial password and follow prompts:  
```$passwd```  
*Note: Be sure your password is safe and correct. Your account will be locked when you input wrong password twice.  
You are not entitled to run at root or sudo.


## Copy the files to your own dir
1.  Assume you have logged in at yourname@nuon-neutrino.ps.uci.edu
2. In your terminal or shell, copy and paste next two lines one by one, replace "stella" with your destination dir:  
```
$cd ../../storage/data/tutorials/  
$cp -r training_files /home/stella
$pip3.6 install tensorflow==1.8.0 absl-py==0.9.0 tensorboard==1.8.0 keras==2.2.1
```
     
## Run Jupyter notebook checking the files and run
Open a new window in your local terminal or shell:  
```
$ssh -L 8080:localhost:8889 you@muon-neutrino.ps.uci.edu`  
$cd ../../  
$python3.6 -m jupyter notebook --no-browser --port=8889
```

In your browser, http://localhost:8080/  
If it prompts a token, look for it in your console, copy and paste it and click "log in".   
Navigate to your destination directory, open the training files as the sequence showing above.  
Click "Not Trust" on the right above first. Then carefully read the comments and codes in them. 

Essential Jupyter shorcuts below:  
```
Ctrl+S - saves the notebook and checkpoint  
cmd + Enter - execute each cell  
h -  shows all keyboard shortcuts  
a -	above new cell  
b -	below new cell  
```
