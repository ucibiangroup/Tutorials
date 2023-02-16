# Tutorials
Tutorials for new group members  

## This repository has three training set, the sequence is:  
1. MnistConvnet.ipynb  
2. Convnets_with_small_datasets(cat_vs_dog).ipynb  
3. Convnets_with_pretrained_datasets(cat_vs_dog).ipynb  


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
```
     
## Run Jupyter notebook checking the files and run
In your terminal or shell:  
```
$ssh -L 8080:localhost:8889 you@muon-neutrino.ps.uci.edu  
$python3.6 -m jupyter notebook --no-browser --port=8889
In your browser, 
http://localhost:8080/
```
