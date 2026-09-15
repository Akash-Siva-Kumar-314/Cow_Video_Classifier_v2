While I was busy making a working model in 'Video_Classification_Study' and 'Cow_Video_Classifier version 1', I missed out on pre processing the data.\
\
This version fixes that and a couple of other fixes.\
\
Pre processing:\
\
<img width="1103" height="142" alt="image" src="https://github.com/user-attachments/assets/95a7fc1f-6ae6-418b-93b5-f099ab75ef06" />\
\
The video data contained 18944 clips in total. A lot were repeating clips in sequential order of naming. Code was written to take 1 out of every 10 clips in sequential order.The reduced dataset contains 1893 clips.\
\
Each clip was 10s long with about 300 frames each. Code was written to reduce the 300 fames to 18 frames equally spaced out.\
\
Now some of the videos had some sort of reflection or glare. I treated them as damaged or unusable videos. Video classification was done to sort out damaged and undamaged clips. 1230 undamaged videos were filtered out.\
\
Sorting:\
\
<img width="1294" height="552" alt="image" src="https://github.com/user-attachments/assets/fa00a397-7f01-4ddc-ad9f-1cf11a9f58a3" />\
\
Training was done to sort videos with a single cow and videos with multiple or plural cows. 'c02.1_Cow_x3d_VideoClassifier_SingularOrPlural_ModelTrain.ipynb' was updated to know how much time it took to train the model, 'c02.1.1_Cow_x3d_VideoClassifier_SingularOrPlural_ModelTrain.ipynb'.\
\
Training was done to sort videos with a single cow according to behaviour. 'c03.1_Cow_x3d_VideoClassifier_EatRestWalk_ModelTrain.ipynb' was updated to know how much time it took to train the model, 'c03.1.1_Cow_x3d_VideoClassifier_EatRestWalk_ModelTrain.ipynb'.\
\
Training was not done to sort plural cows as majority of videos of them are that of 'eating together' and a few where they are 'sitting together' and another few videos of them 'standing together' upon visual examination, very few less than 10.\
\
The figures of this filtering is in the flow chart.\
\
Conclusion:\
\
The training data which I used ranges from 10 to 25 videos for each class, manually picked. With this sorting machine doing good. I can feed the sorted data back to train the model even better.
Studying the Miscellaneous bin also captures types of data that was previously missed out on training the model, and can make the next model training better.



