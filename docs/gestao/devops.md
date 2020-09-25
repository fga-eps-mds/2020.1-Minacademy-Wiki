## Integração Contínua

O projeto é composto por dois repositórios, além da Wiki. O [Backend](https://github.com/fga-eps-mds/2020.1-Minacademy-BackEnd) é desenvolvido na linguagem JavaScript com o framework NodeJS. Os testes são executados por meio das bibliotecas Jest + Supertest.

O [Frontend](https://github.com/fga-eps-mds/2020.1-Minacademy-FrontEnd) também é desenvolvido na linguagem JavaScript. O framework escolhido foi o ReactJS e os testes são executados por meio da bibliotecas Jest + Enzyme.

A ferramenta de CI escolhida foi o GitHub Actions, o qual tem um workflow quase idêntico para Backend e Frontend, considerando que ambos utilizam o comando npm test para execução dos testes. Os testes executam sempre que ocorre um pull request, independentemente da branch.


## Deploy Contínuo

O deploy é realizado automaticamente por meio do GitHub Actions e Packages. Uma vez que a branch develop ou master receba o merge (pois não trabalhamos com commits diretos nessas branchs), o workflow builda as imagens que carregam as dependências e o código adicionado com um Dockerfile voltado para produção. 

Então, essas imagens são enviadas para o Github Packages de cada repositório. As imagens da branch develop recebem a tag homolog pois são consumidas no servidor de homologação, e as imagens da branch master recebem a tag production e são consumidas no servidor de produção.

Por fim, o workflow realiza o acesso remoto ssh nos servidores, baixa as imagens, e inicializa os containers com as novas imagens. Nos servidores, temos apenas variáveis de ambiente e docker-composes com configuraões de homologação/produção. Os servidores estão hospedados na plataforma Digital Ocean.