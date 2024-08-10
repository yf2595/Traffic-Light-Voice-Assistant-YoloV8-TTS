# Traffic-Light-Voice-Assistant

**Overview**
The Traffic Light Voice Assistant project detects traffic lights in video footage, generates descriptive text based on the detected light's color, converts this text into speech, and integrates the generated audio into the video. The resulting video provides not only visual information but also audio feedback regarding the state of traffic lights, making it a useful tool for traffic management and analysis.

**Features**
Traffic Light Detection: Uses YOLOv8 to detect traffic lights in each video frame.
Caption Generation: Creates descriptive text for the detected traffic light's color.
Voice Generation: Converts the descriptive text into speech, creating voice instructions for different traffic light colors.
Audio-Video Synchronization: Integrates the generated audio into the video at precise timestamps, resulting in a video that provides both visual and auditory information.

**Output**
The processed video with voice annotations will be saved as trafic_light_with_sound.avi.
Separate audio files (red.wav, green.wav, yellow.wav) corresponding to each traffic light state are also generated.

**How It Works**
Detection: The YOLOv8 model identifies traffic lights in each video frame.
Captioning: A pre-trained image captioning model generates text descriptions of the traffic light's color.
Speech Generation: The text is converted into speech using a TTS model, creating audio files.
Synchronization: The audio is added to the video at the appropriate times, providing an enhanced video with both visual and auditory information.

Both the TTS and Image-to-Text model are imported from Hugging-Face.
