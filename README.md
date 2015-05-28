# recorder.js
Web Based Video Recorder

Standalone JS includes 

1) MediaStreamRecorder.js
2) RecordRTC.js
3) FileSaver.js
4) Jquery Functions to initiate the recording.

Requires Video resolution as params
var p = {mandatory: {minWidth: 1280,minHeight: 720}};

Initialize Recorder        
var recorderObject = $('video').initRecorder();
$(recorderObject).setParams(p);
$(recorderObject).startRecording();

To stop the recording call PauseRecorder() function which releases the system resources 
and saves the recorded video on your desktop.
