This consists of 2 folders (dynamic2,static) and one mainfinal2.py script the final python script is mainfinal2.py which when executed a live camera will open up on computer and will predict the gestures you do from your left hand the gestures it can predict are of two kinds dynamic and static 

Dynamic gestures :
1.) Hello
2.) Wave (moving hand left-right)

Static gestures:
1.) Thumbs Up
2.) Thumbs Down
3.) Open Palm
4.) Fist (closed palm)
5.) Peace symbol

Approach for static gesture prediction :
1.) Dataset Creation:
Used mediapipe to extract 21 points on hand and stored the coordinates of all points on hand with respect to the wrist point in an csv file 
stored this data for all the gestures (Static\DataSetCreation.py) dataset creation is done using this script
2.) Model Training :
Trained an neural network on the created csv file (Static\datasetShuffle+Ann.ipynb) model is trained by this script(model name is staticGestureANN5)
3.) Integrated the model
