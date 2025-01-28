To build a Python environment do the following

```{sh}
python3.12 -m venv env
source env/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install dvt
python3 -m pip install jupyter
python3 -m pip install matplotlib
python3 -m pip install torch torchvision torchaudio
python3 -m pip install transformers
python3 -m pip install polars pydub
python3 -m pip install onnxruntime
python3 -m pip install sentencepiece protobuf librosa soundfile pyannote.audio
pip freeze > requirements.txt

export PYTORCH_ENABLE_MPS_FALLBACK=1
```

To build the R environment

```{r}
install.packages("renv")
renv::init()
```

And commands for quarto:

```{sh}
quarto preview .
quarto render
```