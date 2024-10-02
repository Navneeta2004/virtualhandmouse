**Virtual Mouse Using Hand Gestures**

This project leverages computer vision and hand gesture recognition to develop a virtual mouse that is operated through hand movements. By capturing video through the webcam, the application detects hand gestures using the MediaPipe library and maps specific hand landmarks to control the mouse cursor, enabling actions like clicking.

**Key Features:**
- **Hand Detection:** The system utilizes the MediaPipe library to detect the user's hand in real time from the webcam feed.
- **Cursor Control:** By monitoring the movement of the thumb and index finger, the application calculates the cursor's position on the screen. The distance between these two fingers influences the speed of cursor movement, with closer or farther positions adjusting the speed.
- **Clicking Mechanism:** When the distance between the thumb and index finger falls within a specified threshold, the program simulates a mouse click action.

**System Requirements:**
- Python 3.x
- OpenCV (cv2)
- Mediapipe
- PyAutoGUI

**Instructions for Use:**
1. Download the source code or clone the repository.
2. Install the necessary Python libraries as outlined in the requirements.
3. Connect a webcam to your computer.
4. Run the `aimouse.py` script.
5. A window will open, displaying the webcam feed along with hand landmarks and the corresponding cursor movements.

**Customization Options:**
- **Cursor Speed:** You can modify the cursor's speed by adjusting the `CURSOR_SPEED` constant.
- **Click Action Threshold:** The threshold for triggering a click, determined by the distance between the thumb and index finger, can be customized by altering the `THUMB_INDEX_DISTANCE_THRESHOLD` constant to suit your needs.

**Known Limitations:**
- The current implementation supports only single-hand control. Multiple hands may cause unpredictable results.
- Hand detection accuracy may be affected by lighting conditions or the orientation of the hand.

**Contributing:**
Contributions are encouraged! Feel free to submit issues or pull requests for improvements or bug fixes.
