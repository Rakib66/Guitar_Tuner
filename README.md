# Guitar_Tuner
The tuner is meant to be simple to understand. Depending on your unique needs, you may further improve and modify it by adding new features, enhancing accuracy, or upgrading the user interface.

The tuner's user interface consists of a title, a set of buttons representing different guitar strings, and two display areas:
1. The "Frequency" area displays the real-time dominant frequency detected from the microphone input.
2. The "Status" area displays the closest guitar string or note based on the detected frequency.

The CSS styles are applied to create a centered and visually pleasing layout.
JavaScript Functions:

1. playNote(audioFile):
This function plays a guitar string sound when called.
It uses the audio element to play pre-recorded audio files associated with each guitar string.

2. updatePitch():
This function is called at regular intervals to analyze the microphone input.
It calculates the dominant frequency using the Web Audio API's

3. AnalyserNode.
The displayed "Frequency" is updated with the detected frequency, and the "Status" is updated with the closest guitar string/note.

4. findDominantFrequency(dataArray, sampleRate):
This utility function calculates the dominant frequency from the frequency data obtained from the microphone input.

5. findClosestNote(frequency):
This utility function determines the closest guitar string/note based on the detected frequency.

6. Web Audio API:
The Web Audio API is utilized to access the user's microphone and analyze the real-time frequency data.
An AnalyserNode is used to process the audio input and extract frequency information.

7. Microphone Access:
The code requests access to the user's microphone using the getUserMedia method, allowing the application to capture audio input.

8. Manual Tuning:
Users can manually play the sound of each guitar string by clicking the corresponding buttons.
The tuner continuously analyzes the microphone input to provide real-time feedback on the detected frequency and the closest guitar string/note.

9. Adjustments:
The tuner is designed to be a simple example. You can enhance and customize it further based on your specific requirements, such as improving accuracy, adding additional features, or refining the user interface.
