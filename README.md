# Online Face Recognition

This repository is a direct application of the Semi-Supervised Learning (SSL) theory studied in my repository called semi-supervised-learning. It consists in an implementation of an online face recognition algorithm. After having taken some pictures of you and your best friend, the algorithm is able to make the difference between the two persons in a changing situation (hence the word 'online').

To play with this game, make sure you have already installed all the required librairies (see file: `requirements.txt`).

To install OpenCV, run:  
``
pip install opencv-contrib-python
``

First, the algorithm must know who are the persons involved in the game. If the two persons are Alice and Bob, then run in your terminal:  
``
sh run.sh --create_profile Alice
``  
The camera is activated and you have to take some pictures of Alice (only) by pressing the touch 's'. When you have enough pictures of Alice (e.g. 15), press the touch 'e' to exit. Do the same procedure for Bob by executing in your terminal the command:  
``
sh run.sh --create_profile Bob
``  
The algorithm is now ready for its task: online face recognition! Run:  
``
sh run.sh --face_reco Alice,Bob
``  
Please note there is no space between Alice and Bob in the above command, just a coma. The algorithm makes the difference between Alice and Bob by framing their faces in two different colors. If you want to take pictures of yourselves, press 's'. If you want to exit, press 'e'. 

Enjoy!

