from openai import OpenAI
client = OpenAI()

audio_file= open("/path/to/file/audio.mp3", "rb")
transcription = client.audio.transcriptions.create(
    model="whisper-1", 
    file=audio_file
)

print(transcription.text)
"Hãy tưởng tượng đến ý tưởng điên rồ nhất mà bạn từng có, và bạn tò mò không biết nó có thể mở rộng thành thứ gì đó lớn hơn gấp 100, 1.000 lần không
from openai import OpenAI
client = OpenAI()

audio_file = open("/path/to/file/speech.mp3", "rb")
transcription = client.audio.transcriptions.create(
    model="whisper-1", 
    file=audio_file, 
    response_format="text"
)

print(transcription.text)
