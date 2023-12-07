<!DOCTYPE html>
<html>
  <body>
    <hr>
    <h1 align="center">Closed Captions Generator</h1>
    <br>
    <p align="center">
      <strong>Closed Captions Generator:</strong> GoogleCloudTwitter2cc
      <br>
      <strong>By: Ryan Hatch</strong>
      <br>
    </p>
    <p align="center">
      <a href="#closed-captions-introduction">Introduction</a> • <a href="#closed-captions-prerequisites">Prerequisites</a> • <a href="#closed-captions-usage">Usage</a> • <a href="#closed-captions-dependencies">Dependencies</a> • <a href="#closed-captions-example">Example</a><h2></h2>
    <p align="center">
      <strong>Simple Audio To CC Generator:</strong> Twitter2CC
      <br>
    </p>
    <p align="center">
      <a href="#simple-closed-captions-introduction">Introduction</a> • <a href="#simple-closed-captions-prerequisites">Prerequisites</a> • <a href="#simple-closed-captions-usage">Usage</a> • <a href="#simple-closed-captions-dependencies">Dependencies</a> • <a href="#simple-closed-captions-example">Example</a>
    </p>
    <hr><br>
    <p align="center"> &copy; 2023 Ryan Hatch <br> All Rights Reserved. </p>
    <br>
    <h1 align="center"><strong>GoogleCloudTwitter2cc</strong></h1>
    <!-- Closed Captions Section -->
    <h2 id="closed-captions-introduction">Introduction</h2>
    <p> This Python script allows you to generate closed captions for audio files using the Google Cloud Speech-to-Text API.<br>Closed captions are essential for accessibility and can enhance the accessibility of audio content.</p>
    <h2 id="closed-captions-prerequisites">Prerequisites</h2>
    <p> Before using this script, make sure to:</p>
    <ol>
      <li>Replace <code>path_to_your_audio_file.wav</code> with the path to your audio file.</li>
      <li>Set up Google Cloud credentials on your machine where the script will be run. You can find information on how to set up Google Cloud API credentials <a href="https://cloud.google.com/docs/authentication/getting-started">here</a>.</li>
    </ol>
    <h2 id="closed-captions-usage">Usage</h2>
    <p> Follow these steps to use the script:</p>
    <ol>
      <li>Ensure the prerequisites are met and requirements are installed.</li>
      <li>Run the script.</li>
      <li>The script will transcribe the audio file and print the results, including word-level timestamps.</li>
    </ol>
    <h2 id="closed-captions-dependencies">Dependencies</h2>
    <p> - <code>google-cloud-speech:</code> The script uses the Google Cloud Speech-to-Text API for audio transcription.</p>
    <h2 id="closed-captions-example">Example</h2>
    <p> Example code for the closed captions script:</p>
    <code>       from google.cloud import speech_v1p1beta1 as speech<br>
        from google.cloud.speech_v1p1beta1 import enums<br>
        from google.cloud.speech_v1p1beta1 import types<br>
        import io<br><br></code>
        <br><br>
    <code>       # ...<br><br>
        # Transcribe the audio file<br>
        response = client.recognize(config=config, audio=audio)</code>
    <h2></h2>
    <br><br>
    <h1 align="center"><strong>Simple Audio To CC</strong></h1>
    <!-- <br> -->
    <!-- simple Closed Captions Section -->
    <h2 id="simple-closed-captions-introduction">Introduction</h2>
    <p> This Python script provides a simple method to generate closed captions from an audio file in MP3 format.<br>It converts the MP3 file to WAV format and then transcribes the audio to text.</p>
    <h2 id="simple-closed-captions-prerequisites">Prerequisites</h2>
    <p> Before using this script, make sure to:</p>
    <ol>
      <li>Replace <code>SBFTwitterSpace.mp3</code> with the path to your MP3 audio file.</li>
    </ol>
    <h2 id="simple-closed-captions-usage">Usage</h2>
    <p> Follow these steps to use the script:</p>
    <ol>
      <li>Ensure the prerequisites are met.</li>
      <li>Run the script.</li>
      <li>The script will transcribe the audio and print the results.</li>
    </ol>
    <h2 id="simple-closed-captions-dependencies">Dependencies</h2>
    <p> - <code>pydub:</code> The script uses <code>pydub</code> to convert MP3 files to WAV format.<br>- <code>speech_recognition:</code> The script uses the <code>speech_recognition</code> library to perform audio transcription.</p>
    <h2 id="simple-closed-captions-example">Example</h2>
    <p> Example code for the simple closed captions script:</p>
    <code>      from pydub import AudioSegment<br>
        import speech_recognition as sr<br><br></code><br><br>
    <code>      # Convert mp3 file to wav<br>
        mp3_file_path = <code>SBFTwitterSpace.mp3</code><br>
        wav_file_path = <code>SBFTwitterSpace.wav</code><br><br>
        # ...<br><br></code><br><br>
    <code>      # Recognize (convert from speech to text)<br>
        try:<br>
            text = recognizer.recognize_google(audio_data)<br>
            print(text)<br>
        except sr.UnknownValueError:<br>
            print("Speech Recognition could not understand audio")<br>
        except sr.RequestError as e:<br>
            print(f"Could not request results from Google Speech<br> Recognition service; {e}")<br><br></code>
    <h2 id="contact">Contact</h2>
    <p> For any inquiries or suggestions, please contact me at <a href="mailto:ryan@rshatch.com">ryan@rshatch.com</a>.</p>
  </body>
</html>
