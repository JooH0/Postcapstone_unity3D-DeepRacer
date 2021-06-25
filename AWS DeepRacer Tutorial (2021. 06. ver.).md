# AWS DeepRacer Tutorial (2021. 06. ver.)

---

## 1. Enter AWS website to prepare for DeepRacer training.

https://console.aws.amazon.com/deepracer/home?region=us-east-1#welcome

**1. You can see the AWS DeepRacer homepage through the link above.**

![image-20210625165231103](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625165231103.png)



**2. Click on the banner on the left side of the window.**

![image-20210625165618410](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625165618410.png)



**3. You can see several menus for reinforcement Learning.**

![image-20210625180006872](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625180006872.png)

---

**Get started** : you can create model.

**Your models** : you can see the models you made before.

**Your garage** : you can configure your vehicle with one or more sensors, choose a neural 			            network topology, and customize the action space to meet your racing criteria.

---



## 2. Create your reinforcement learning model

**1. Click the "Get started" for creating your custom model**

![image-20210625180145025](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625180145025.png)

---

**start the course :** You can get basic reinforcement learning knowledge and general 							      information about DeepRacer (It takes about 10 minutes).

---



**2. Create your custom model** (Follow the steps provided by AWS)

Enter the name of your model.

![image-20210625181544680](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625181544680.png)

---



**3. Choose a course you want to simulate.**

![image-20210625182043051](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625182043051.png)

**If you try training for the first time, "Oval Track" is recommended.**

![image-20210625182540680](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625182540680.png)

---



**4. Race type & Training algorithm**

![image-20210625183758381](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625183758381.png)

___

You can choose three types of racing. Depending on the race type, you can train with different goals. 

- **Time trial**: race against the clock on an unobstructed track and aim to get the fastest lap time possible.
- **Object avoidance**: race against the clock on a track with stationary obstacles and aim to get the fastest lap time possible.
- **Head-to-head racing**: race against one or more other vehicles on the same track and aim to cross the finish line before other vehicles.

AWS provides PPO and SAC as training algorithms, and if you want to change the hyperparameters, click "Hyperparameters" below in your screen.

if you want to get more information about PPO and SAC, click the link below.

https://docs.aws.amazon.com/deepracer/latest/developerguide/deepracer-how-it-works-reinforcement-learning-algorithm.html

---



**5. Agent** (Choose a vehicle you have.)

![image-20210625183850343](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625183850343.png)



**6. Reward function**

![image-20210625184330224](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625184330224.png)

---

You can edit the reward function code. It will be used to train your model.  If you want to get some example code, click the "Reward function examples". It provides some reward functions for examples and you can train your model with them.

If you want to get some information about "Reward function examples", visit the link below.

https://docs.aws.amazon.com/deepracer/latest/developerguide/deepracer-reward-function-examples.html

If you want to know about the input parameters of AWS DeepRacer reward function, visit the link below.

https://docs.aws.amazon.com/deepracer/latest/developerguide/deepracer-reward-function-input.html

---



**7. Stop conditions**

you can set "Maximum time" for stop conditions.

![image-20210625185250983](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625185250983.png)

---



## 3. Train your model & Evaluate.

![image-20210625185641940](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625185641940.png)

You can see this screen if you've followed the steps well. It takes time to create a model.

Training will start automatically when the initialization is complete.

---



**1. Training monitor**

![image-20210625190426294](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625190426294.png)

---

You can only watch simulation videos when training is in progress.

As the training progresses, the left graph is drawn. The graph includes three things below.

- Average reward (Training) , green color
- Average percentage completion (Training), Blue color
- Average percentage completion (Evaluating), Red color

You can judge whether the model is well trained and stop training early through reward graphs.

---



**2. Evaluate your model**

if your model have finished training, you can evaluate the model.

![image-20210625191410043](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625191410043.png)

---



## 4. Apply physical DeepRacer.

Click "Download phsical car model" to download your trained weight file.

The trained model can be applied to real DeepRacer.

![image-20210625192325393](C:\Users\rlawn\AppData\Roaming\Typora\typora-user-images\image-20210625192325393.png)



## 5. Connecting the DeepRacer to your computer.



