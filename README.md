# AudioRecorder

An audio recorder written in Javascript and HTML. The main audio recorder is in the file 'AUAudioRecorder.js' which contains the AUAudioRecorder object. To see a very simple example of the audio recorder at work, navigate to the 'RecorderTester.html' file in the Example folder.

# Methods
- **startRecording()**: Starts the recording process. If the program does not have permission to access the computer’s microphone yet, it will ask the user for it.
- **stopRecording()**: Stops recording and saves the recorded audio into a variable with a file type that can be specified by another method.
- **play()**: Plays the recorded audio in the browser.
- **pause()**: Pauses the audio that is playing. when the play button is clicked again the audio will resume from where it was.
- **stop()**: Stops the audio from playing and sends it back to the beginning.
- **requestPermission()**: Asks the user for permission to access the computer’s microphone. This is automatically called by the startRecording() method if permission was not already given, however permission can be requested beforehand by calling this method.
- **getRecording()**: Returns an audio object that contains the recorded audio.


# How To
- Step 1: Clone the repository onto your computer.
- Step 2: Drag the 'AUAudioRecorder.js' file into your project directory.
- Step 3: Add the script to your HTML file like so: 
```html
<script src=“(path to the file that you put in your project directory)”></script>
```
- Step 4: Assuming you have already created buttons in your HTML file and already have your own Javascript file for your webpage, you can create a new AUAudioRecorder object and call method from it when buttons are clicked.
```javascript
var audioRec = new AUAudioRecorder();


audioRec.startRecording();
audioRec.stopRecording();
audioRec.play();
audioRec.pause();
audioRec.stop();
audioRec.getRecording();

```


- Year: 2016
- Languages: HTML, Javascript
- Programmer: Adeola Uthman
