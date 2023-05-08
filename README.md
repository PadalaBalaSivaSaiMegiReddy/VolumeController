
# Hand Gesture Volume Control

This code is used to control the volume of the computer using hand gestures. It uses OpenCV and MediaPipe to detect the hand/finger position, and then calculates the distance between the tips of the index finger and thumb to control the volume.

## Prerequisites
To run this code, the following packages need to be installed:

1.OpenCV

2.Mediapipe

3.numpy

4.pycaw






## Usage/Examples

```
1.Import all the required packages.

2.Initialize the camera and the hand/finger detection using the cv2.VideoCapture() and mpHands.Hands() functions.

3.Access the speaker through the pycaw library and get the volume range.

4.Capture the video from the camera using the cap.read() function and convert it to RGB using cv2.cvtColor().

5.Process the image to get the hand/finger landmarks using hands.process().

6.Loop through the list of all the detected hands to get the information of each hand's corresponding flag bit.

7.Get the finger joint points and add them to an empty list lmList.

8.Draw the landmarks and connections using mpDraw.draw_landmarks().

9.Calculate the distance between the tips of the index finger and thumb using hypot().

10.Convert the hand range to the volume range using np.interp().

11.Set the volume using volume. 

12.SetMasterVolumeLevel().

13.Create a volume bar for the volume level 

14.using cv2.rectangle() and cv2.putText().

15.Show the video using cv2.imshow() and exit the loop when spacebar is pressed.
Release the camera and close the window using cap.release() and cv2.destroyAllWindows().
```


## License

[MIT](https://choosealicense.com/licenses/mit/)

