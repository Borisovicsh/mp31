# mp31
music convert
# Code for MP3 Converter using pydub
from pydub import AudioSegment

# Load the audio file
input_file_path = "input_audio.wav"
output_file_path = "output_audio.mp3"

audio = AudioSegment.from_wav(input_file_path)

# Export as MP3
audio.export(output_file_path, format="mp3")

print(f"Conversion complete. MP3 file saved at {output_file_path}")
