# Speech-Recognition-System

This is an isolated word recognition system which takes input from user, perform some pre-processing steps, extract features 
then it goes through the classification step and use the prediction in a specific program.

> 1- The pre-processing steps are silence removal, noise reduction and adjusting audio size. </br>
> 2- The extraction technique used is MFCC (Mel Frequency Cepsteral Coefficient). </br>
> 3- The classification is done by using ANN and CNN for each application to compare the performance of each model. </br>
> 4- The applications applied are a command system and a numbering system. </br>

## Command System
> The program takes the input as a spoken word from the user Using the Directions Model with the words [Up, Down, Left, Right, Stop] then process it to be detected.
  After detection it drives the object to the certain needed direction. </br>
  
  #### Conclusion
  > using a CNN classifier and MFCC features. But unfortunately, although the proposed system could detect all five commands with high accuracy, it causes a slight         slowness in the game. For example, the voice command did not take long to be detected but took about a second to be fed into the game and processed by the game           function. As a result, the user should wait until the action is taken on the screen before entering the next command.
  
## Number System
> This progaram is used by speaking each number individually from 0 to 9, after the output is shown on the screen, we speak the following number, and the output will be   updated. </br>

  #### Conclusion
  > using ANN model which had a very good theoretical accuracy but when in real time it showed a very bad performance which we tried to improve by adding more hidden       layers, but its performance was still poor.</br>
  At this point I decided to implement a CNN model which had an excellent theoretical accuracy, and the performance was satisfying as CNN can extract the features and
  recognize patterns of the input data better than ANN when dealing with larger number of classes which are 10 classes in our case, so we decided to work with the CNN     model as it was the best fit for this system.
