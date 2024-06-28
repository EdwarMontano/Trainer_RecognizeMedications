# README

Welcome to the Trainer_RecognizeMedications project!

## Description

This project aims to train a machine learning model to recognize medications from text data. It utilizes natural language processing techniques and a labeled dataset to build an accurate medication recognition system.

## Installation

### Instalación con pyenv y poetry
es el modo difícil  de levantar el proyecto  pero nos sirve para habilitar las opciones de debug mas fácil. recuerde instalar un motor de mongo para la bd.
```bash
pyenv versions #opcional: sirve para comprobar si la version de python que necesitamos ya se encuentra descargada
pyenv install --list #opcional: sirve para listar los versiones disponible por pyenv
pyenv install 3.10.12 
pip install poetry #Solo en windows
```

```bash
poetry --version
poetry env info
poetry env use $(pyenv which python)
poetry env info # la version de python debe coincidir 
poetry shell 
poetry install
poetry show # dependencias instaladas == pip list
poetry add [dependecias]
```
🚫 :sos: Si al realizar la instalación de las dependencia se presenta un error. Elimanar el archivo poetry.lock y ejecutar el siguiente comando

## Usage

After training the model, you can use it to recognize medications in text by running the `predict.py` script. Make sure to provide the necessary input data in the correct format.

```python
python predict.py --input "This is a sample text containing medication names like Aspirin and Ibuprofen."
```

## Contributing

Contributions are welcome! If you have any ideas or improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
