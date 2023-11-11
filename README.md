# text-to-speech
from gtts import gTTS
from IPython.display import Audio

text = "my name is Kwanda, i schooled in Bauchi and i am an engineer."

# Create a gTTS object
tts = gTTS(text=text, lang='en')

# Save the speech as an audio file
tts.save("output.mp3")

# Display the audio file
Audio("output.mp3", autoplay=True)
