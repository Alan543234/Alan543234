import gtts
from gtts import gTTS
import os

def text_to_audio(text, lang='es'):
    tts = gTTS(text=text, lang=lang, slow=False)
    tts.save("output.mp3")
    os.system("start output.mp3")

text = "Hello, world!"
text_to_audio(text)
