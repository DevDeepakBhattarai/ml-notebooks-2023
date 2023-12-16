# ML & Deep Learning Training Notebooks (2023)

Archive of original deep learning and NLP experiments built and trained in Google Colab in late 2023. Each notebook retains its original 2023 Colab cell execution timestamps in its metadata and opens directly in Google Colab via the badges below.

## Notebooks

| Date (2023) | Notebook | Summary | Colab |
| --- | --- | --- | --- |
| Nov 2023 | [`Transformer_Image_Model.ipynb`](./Transformer_Image_Model.ipynb) | Custom image captioning architecture built from scratch in TensorFlow/Keras: frozen VGG16 visual encoder + 5-block Transformer Decoder (`d_model=512`, `num_heads=8`, custom causal & cross-attention, sinusoidal `PositionalEncoding`), custom Flickr30k (`158,915` caption pairs) batch generator, multi-epoch checkpointing, and autoregressive caption inference. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DevDeepakBhattarai/ml-notebooks-2023/blob/main/Transformer_Image_Model.ipynb) |
| Nov 2023 | [`ImageCaptioning_CNN_LSTM.ipynb`](./ImageCaptioning_CNN_LSTM.ipynb) | Earlier CNN + LSTM baseline for Flickr30k image captioning (`Conv2D`/`MaxPool2D` encoder + `Embedding`/`LSTM` sequence decoder with custom tokenization and checkpointing). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DevDeepakBhattarai/ml-notebooks-2023/blob/main/ImageCaptioning_CNN_LSTM.ipynb) |
| Dec 2023 | [`Voice_Communication_Coach.ipynb`](./Voice_Communication_Coach.ipynb) | End-to-end spoken communication practice pipeline chaining Whisper (`openai/whisper-medium`) STT, quantized Mistral-7B-Instruct (`CTransformers` + `LangChain` conversation memory), Suno Bark TTS, and a Gradio microphone UI. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DevDeepakBhattarai/ml-notebooks-2023/blob/main/Voice_Communication_Coach.ipynb) |
| Sep 2023 | [`CNN.ipynb`](./CNN.ipynb) | TensorFlow/Keras CNN architecture on MNIST plus pooling-based image downscaling experiments. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DevDeepakBhattarai/ml-notebooks-2023/blob/main/CNN.ipynb) |

## Notes

- Large trained `.keras` checkpoint weights (~240 MB to ~740 MB each) and raw datasets (Flickr30k) are excluded from Git; the notebooks include the full data prep, model definitions, training loops, and saved inference outputs.
- Originally authored in Google Colab (Sep to Dec 2023) and synced here so each notebook is directly linkable and runnable in Colab.
