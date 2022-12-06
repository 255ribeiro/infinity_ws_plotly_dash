# Gráficos Interativos com Python, Plotly e Dash

<img src=" ./figs/logo_visual_header.png" >

## Stack

* `Python` - Conhecimento básico da linguagem incluindo:
    * `Listas`
    * `Dicionários`
    * `Funções`
    * `Ambientes virtuais`
* `Numpy` - Pacote básico de programação científica mais utilizado na distribuição CPython
* `Pandas` - Pacote de análise e manipulação de dados (depende do Numpy)
* `Plotly` - Pacote de geração de gráficos 
* `Flask` - [Opcional] Web framework que serve de base para Dash
* `Dash` - Cria aplicativos web interativos com os gráficos gerados pelo Plotly


## Árvore de dependências

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

## Objetivos



