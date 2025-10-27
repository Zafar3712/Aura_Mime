# Aura_Mime
End-to-End Speech Emotion Recognition and Emotion-Aware Voice Synthesis



This project presents an integrated multimodal emotion-aware speech synthesis pipeline that transforms a user's voice recording into emotionally expressive speech while preserving the original speaker’s voice characteristics. The system combines audio-based emotion recognition, speech-to-text transcription, text-based emotion analysis, and emotion-conditioned voice synthesis into a unified workflow. The input audio is first segmented using adaptive silence detection. Each segment is then analyzed multimodally: a fine-tuned Hugging Face model detects the audio emotion, while OpenAI Whisper generates a transcription, which is in turn analyzed by a DistilRoBERTa-based text emotion classifier. Subsequently, the transcribed text and the primary detected audio emotion guide the generation of expressive audio through Coqui TTS, which clones the speaker’s voice and applies the corresponding emotional tone. The resulting emotional speech segments are concatenated to produce a coherent, expressive audio output. This work demonstrates a practical framework for emotionally enhanced speech synthesis, with potential applications in human-computer interaction, voice assistants, affective computing, and personalized audio content generation.

