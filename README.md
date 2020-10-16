# Wiki

Este repositório contém os **documentos** e ferramentas para alimentar a wiki em https://github.com/fga-eps-mds/2020.1-Minacademy-Wiki/, pertencente ao grupo Minacademy de EPS/MDS em 2020/1.

## Requisitos 
Recomendamos rodar o repositório localmente e checar se as alterações não quebraram a Wiki. Para isso você precisa:

- Ter o Docker instalado. No caso do Ubuntu, [clique aqui](https://docs.docker.com/engine/install/ubuntu/) para ver as instruções.
- **OU** ter Mkdocs instalado. [Clique aqui](https://www.mkdocs.org/) para ver as instruções.


## Como Rodar
Este repositório utliza o Mkdocs para testes locais. Você instalar em sua máquina e utilizar os comandos padrões do mkdocs. Porém, para facilitar o processo nós fornecemos um Makefile que utiliza o Docker.

* Apenas no primeiro uso do repositório, compile a imagem com:<br>
```make build```

* Para rodar o repositório rode o comando abaixo e então acesse localhost na porta 8000.<br>
```make run```

Agora você pode alterar os arquivos *md* e o *mkdocs.yml* e ver as alterações aparecerem em tempo real no seu browser. Para mais comandos leia nosso Makefile ou rode seus próprios comandos.