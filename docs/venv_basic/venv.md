# Criando um ambiente virtual

## Utilizando o pip e venv

### Crie o ambiente virtual 

```shell

python -m venv .venv

```

dependendo das configurações do seu sistema operacional, pode ser necessário executar o python como python3

```shell

python3 -m venv .venv

```

```shell

pip install pandas dash

```

## Exportando requirements.txt

```shell

pip freeze >> requirements.txt

```

# Utilizando o Poetry


## Para instalar, veja as informações na documentação

[documentação](https://python-poetry.org/docs/)

## Configurando para criação de ambiente virtual na pasta do projeto

```shell

poetry config virtualenvs.in-project true


```

## Iniciando o Poetry

```shell

poetry init <nome da pasta>

```

ou

```shell

poetry init .

```

## Adicionando pacotes


```shell

poetry add dash

poetry add pandas

```

## Instalando ambiente Poetry


```shell

poetry install

```

## Exportando o arquivo requirements.txt

### Exportando com hashes

```shell

poetry export -f requirements.txt -o requirements.txt

```

ou

```shell

poetry export  --format=requirements.txt > requirements.txt

```


### Exportando sem hashes


```shell

poetry export  --without-hashes -f requirements.txt -o requirements.txt

```

ou

```shell

poetry export --without-hashes --format=requirements.txt > requirements.txt

```

ou

```shell
poetry export  --without-hashes -f requirements.txt > requirements.txt

```


