# Preserving-Speaker-Identity-In-Multilingual-Translation
Preserving Speaker Identity In Multilingual Translation using fine-tuned Whisper, XTTS V2, and Marian NMT
The surge in globalization and the unprecedented rise in virtual collaboration
in academia and industries alike has ushered in an era where real-time multi-
lingual communication is no longer optional but essential. Yet current speech
translation technologies force an unnatural choice: either communicate through
impersonal, synthetic voices or lose the immediacy of real-time interaction. While
separate solutions exist for machine translation and voice preservation, main-
taining a speaker’s identity and voice characteristics across languages remains an
unsolved challenge. This project aims to bridge this gap by combining state-of-
the-art Neural Machine Translation systems with advanced voice cloning systems,
focusing specifically on English-French translation. The proposed system utilizes
Marian MT for translation and XTTS for voice synthesis, with OpenAI’s Whis-
per model handling the speech recognition component. Each of the three models
in the pipeline were further finetuned with specialized datasets to reduce errors
and optimize performance for our specific use case. OpenAI’s Whisper-tiny model
was finetuned on a section of the Librispeech dataset, achieving an overall WER
score of 0.20 and CER score of 0.05, outperforming the base model. Marian MT,
utilized for Neural Machine Translation was finetuned on OPUS dataset, result-
ing in an improved BLEU score of 40.38%. XTTS model was finetuned on Mozilla
Common Voice French dataset, achieving improved scores compared to the base
model. The enhanced performance metrics across ASR, translation, and voice
synthesis components demonstrate the effectiveness of our integrated approach in
preserving both linguistic accuracy and speaker identity. Finally, Mlflow is used
to build these experiments, register, evaluate, and serve the most performant
versions of these models.
