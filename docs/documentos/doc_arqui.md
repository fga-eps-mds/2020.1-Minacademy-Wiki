# _Histórico de Revisão_

|Data|Versão|Descrição|Autor|
|----|------|---------|-----|
|03/09/2020| 0.1.0| Inserção dos tópicos de "Introdução" e "Representação da Arquitetura" | Estevão |
|03/09/2020| 0.2.0| Inserção do tópico "Tamanho e Desempenho" | Eduardo |
|03/09/2020| 0.3.0| Inserção do tópico "Metas e Restrições da Arquitetura" | Eduardo |
|04/09/2020| 0.3.1| Correções de formatação de Referência e Inserção de imagens nos tópicos "2.1.3 Representação arquitetural da camada de apresentação" e "2.4.Diagrama de Relações" | Estevao|

# _1.Introdução_

## _1.1.Finalidade_
Este documento tem como finalidade apresentar a arquitetura do projeto <nome_do_projeto>,oferecendo uma visão geral arquitetural do sistema que será implementado, possibilitando assim que os envolvidos no projeto tenham conhecimento de como a aplicação será subdivida e quais serão as funções de cada componente.

## _1.2.Escopo_
Este documento apresenta as características arquiteturais do projeto <nome_do_projeto>, expondo detalhadamente as soluções arquiteturais idealizadas e estabelecidas para o projeto, de modo a ser utilizado como base para a edificação do projeto pelos desenvolvedores designados para o projeto.

## _1.3.Definições, acrônimos, abreviações_
|Definições/Acrônimos/Abreviações| Significado|
|--------------------------------|------------|
|MERN|MongoDB, Express, React, Node|
|MC| Model Controller|
|UI|User Interface (Interface do Usuário)|
|GUI|Graphical User Interface|
|MVC| Model View Controller|


## _1.4.Referências Bibliográficas_
[1]_Modelo em três camadas_. Disponível em <https://pt.wikipedia.org/wiki/Modelo_em_tr%C3%AAs_camadas>.Acesso em 03 de Setembro de 2020.

[2]_MERN Stack_. Disponível em <https://www.mongodb.com/mern-stack>. Acesso em 02 de Setembro de 2020

[3]_Tutorial: Introdução ao React_. Disponível em <https://pt-br.reactjs.org/tutorial/tutorial.html>. Acesso em 03 de Setembro de 2020

[4]_Redux Essentials, Part 1: Redux Overview and Concepts_. Disponível em <https://redux.js.org/tutorials/essentials/part-1-overview-concepts>. Acesso em 03 de Setembro de 2020.

[5]_Node.js – O que é, como funciona e quais as vantagens_. Disponível em <https://www.opus-software.com.br/node-js/>. Acesso em 04 de Setembro de 2020.

[6]_Express Framework web rápido, flexível e minimalista para Node.js_. Disponível em <https://expressjs.com/pt-br/>. Acesso em 03 de Setembro de 2020.

[7]_MongoDB_. Disponível em <https://pt.wikipedia.org/wiki/MongoDB>. Acesso em 03 de Setembro de 2020.

[8]_Elm architecture with React + Redux + Redux-loop_. Disponível em <https://smallbusinessforum.co/elm-architecture-with-react-redux-redux-loop-645a67070b1a>. Acesso em 03 de Setembro de 2020.

[9]_MVC_. Disponível em <https://pt.wikipedia.org/wiki/MVC#:~:text=MVC%20%C3%A9%20o%20acr%C3%B4nimo%20de,a%20apresenta%C3%A7%C3%A3o%20dos%20dados%20e>. Acesso em 04 de Setembro de 2020.

[10]_diag-arqui_. Disponível na pasta do projeto em <coloco o nome endereço do repositório>

## _1.5.Visão Geral_

|Tópico| Descrição|
|------|----------|
|Introdução| Fornece uma visão geral do documento inteiro, descrevendo informações sobre a sua finalidade|
|Representação Arquitetural| Traz o detalhamento da arquitetura de software do sistema para melhor entendimento de sua estrutura e funcionamento. Além de apresentar o modo como ela está sendo representada.|
|Metas e Restrições| Detalha os requisitos e objetivos do software que têm algum impacto sobre a arquitetura. Ela também captura as restrições especiais que podem ser aplicáveis.|
|Visão lógica| Retrata as partes relevantes concernente à arquitetura do modelo de design. |
|Visão de implementação| Descreve a estrutura geral do modelo de implementação, a divisão do software em camadas e os subsistemas no modelo de implementação e todos os componentes significativos do ponto de vista da arquitetura.|

# _2.Representação da Arquitetura_
A arquitetura do projeto <nome_do_projeto> é composta por frontend e backend desacoplados, cada um possuindo seu próprio repositório. Por consequência desse desacoplamento, o risco de uma mudança em um dos dois não causará efeitos colaterais na implementação do outro. O modelo de arquitetura que será utilizada é Modelo em 3 Camadas(3-Tier), expecificamente o modelo MERN Stack.

O modelo 3-Tier, derivado do modelo 'n' camadas, organizando a aplicação nas camadas de apresentação, de négocio e de dados. A separação em camadas lógicas torna os sistemas mais flexíveis, permitindo que as partes possam ser alteradas de forma independente. As funcionalidades da camada de negócio podem ser divididas em classes e essas classes podem ser agrupadas em pacotes ou componentes, reduzindo as dependências entre as classes e pacotes; podem ser reutilizadas por diferentes partes do aplicativo e até por aplicativos diferentes. O modelo de 3 camadas tornou-se a arquitetura padrão para sistemas corporativos com base na Web.[1]

MERN é o acrônimo para MongoDB, Express, React, Node, nome das quatro tecnologias principais que compõem a stack. A arquitetura MERN permite que você construa facilmente uma arquitetura de 3 camadas (front-end, back-end, banco de dados) inteiramente usando JavaScript e JSON[2].

## _2.1.Camada de apresentação (Front-end)_
É a chamada GUI, ou simplesmente interface. Esta camada interage diretamente com o usuário, é através dela que são feitas as requisições como consultas, por exemplo. Nessa camada são utilizadas as tecnologias React em conjunto com a Redux.[1]

### _2.1.1 React_
O React é uma biblioteca JavaScript declarativa, eficiente e flexível para criar interfaces com o usuário. Ele permite compor UIs complexas a partir de pequenos e isolados códigos chamados “componentes”[3].

### _2.1.2 Redux_
Redux é um padrão e biblioteca para gerenciar e atualizar o estado do aplicativo, usando eventos chamados "ações". Ele serve como um armazenamento centralizado para o estado que precisa ser usado em todo o seu aplicativo, com regras que garantem que o estado só possa ser atualizado de maneira previsível.[4]

### _2.1.3 Representação arquitetural da camada de apresentação_
![Representação-Arquitetura-React-Redux](https://miro.medium.com/max/512/1*Or0o-_dFsZe1ahMAC2yLZQ.png)[8]

## _2.2.Camada de negócio (Back-end)_
Também chamada de lógica empresarial, regras de negócio ou funcionalidade. É nela que ficam as funções e regras de todo o negócio. Não existe uma interface para o usuário e seus dados são voláteis[1]. Nessa camada são utilizadas as tecnologias Node em conjunto com Express

### _2.2.1 Node_
O Node.js pode ser definido como um ambiente de execução Javascript server-side.Isso significa que com o Node.js é possível criar aplicações Javascript para rodar como uma aplicação standalone em uma máquina, não dependendo de um browser para a execução[5]. Na aplicação o node fará uso da arquitura MC, proveniente da arquitetura MVC, excluindo a parte V que lida com a interface do usuário, a tecnologia React será responsavel por essa parte.

MVC é o acrônimo de Model-View-Controller (em português: Arquitetura Modelo-Visão-Controle - MVC) é um padrão de projeto de software,ou padrão de arquitetura de software, focado no reuso de código e a separação de conceitos em três camadas interconectadas, onde a apresentação dos dados e interação dos usuários (front-end) são separados dos métodos que interagem com o banco de dados (back-end).[9]

### _2.2.2 Express_
O Express é um framework para aplicativo da web do Node.js mínimo e flexível que fornece um conjunto robusto de recursos para aplicativos web e móvel[6].

## _2.3.Camada de Dados_
É composta pelo repositório das informações e as classes que as manipulam. Esta camada recebe as requisições da camada de negócios e seus métodos executam essas requisições em um banco de dados[1]. Nessa camara é utilizada a tecnologia MongoDB.

### _2.3.1 MongoDB_
MongoDB é um software de banco de dados orientado a documentos livre, de código aberto e multiplataforma, escrito na linguagem C++. Classificado como um programa de banco de dados NoSQL, o MongoDB armazena dados em documentos do tipo JSON. Suas características permitem com que as aplicações modelem informações de modo muito mais natural, pois os dados podem ser aninhados em hierarquias complexas e continuar a ser indexáveis e fáceis de buscar[7].
    
## _2.4.Diagrama de Relações_
![Diagrama-de-Arquitetura-de-Software](./imagens/diag-arqui.png)[10]