To build a Python environment do the following

```{sh}
python3 -m venv env
source env/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install dvt
python3 -m pip install jupyter
python3 -m pip install matplotlib
pip freeze > requirements.txt
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