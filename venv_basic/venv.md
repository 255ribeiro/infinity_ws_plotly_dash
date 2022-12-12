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

### Exportando requirements.txt

```shell

pip freeze >> requirements.txt

```

## Utilizando o Poetry


### Para instalar, veja as informações na documentação

[Documentação](https://python-poetry.org)

[Instalação](https://python-poetry.org/docs/#installation)

### Configurando para criação de ambiente virtual na pasta do projeto

```shell

poetry config virtualenvs.in-project true


```

### Iniciando o Poetry

```shell

poetry init <nome da pasta>

```

ou

```shell

poetry init

```

### Adicionando pacotes


```shell

poetry add dash

poetry add pandas

```

### Instalando ambiente Poetry


```shell

poetry install

```

### Exportando o arquivo requirements.txt

#### Exportando com hashes

```shell

poetry export -f requirements.txt -o requirements.txt

```

ou

```shell

poetry export  --format=requirements.txt > requirements.txt

```


#### Exportando sem hashes


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



### Árvore de dependências

```shell

(.venv) poetry show -t --no-dev

dash 2.7.0 A Python framework for building reactive web-apps. Developed by Plotly.
|-- dash-core-components 2.0.0
|-- dash-html-components 2.0.0
|-- dash-table 5.0.0
|-- flask >=1.0.4
|   |-- click >=8.0 
|   |   `-- colorama * 
|   |-- itsdangerous >=2.0
|   |-- jinja2 >=3.0
|   |   `-- markupsafe >=2.0
|   `-- werkzeug >=2.2.2
|       `-- markupsafe >=2.1.1 (circular dependency aborted here)
`-- plotly >=5.0.0
    `-- tenacity >=6.2.0
pandas 1.5.2 Powerful data structures for data analysis, time series, and statistics
|-- numpy >=1.21.0
|-- numpy >=1.23.2
|-- python-dateutil >=2.8.1
|   `-- six >=1.5
`-- pytz >=2020.1

```

