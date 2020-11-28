# Teste Funcional

O teste funcional visa verificar a aceitabilidade dos dados, do processamento, da resposta do mesmo e a implementação apropriada das regras de negócio. Esse teste visa verificar o sistema através da interação da Interface Gráfica de Usuário(GUI) e analisar as saídas e resultados dessa interação.
Para realizar o teste funcional foi utilizado o **Cypress**, um framework de testes automatizados end-to-end. Como os repositórios do backend e frontend são separados, não foi possível colocar na integração contínua(CI), porém é possível rodar localmente rodando o script “npm run cypress”. Os testes podem ser visualizados nos gif’s abaixo.

## Testes executados no projeto

!['Teste de Aprendiz'](https://github.com/fga-eps-mds/2020.1-Minacademy-Wiki/blob/102-testes-funcionais/docs/produto/testesFuncionais/gifs/Learner.gif)

- Fazer login com usuário não cadastrado
- Fazer login com usuário do tipo aprendiz
@@ -37,15 +37,15 @@ Para realizar o teste funcional foi utilizado o **Cypress**, um framework de tes
  - Acessar aba de certificados
  - Verificar certificados

!['Teste de Mentor'](https://github.com/fga-eps-mds/2020.1-Minacademy-Wiki/blob/102-testes-funcionais/docs/produto/testesFuncionais/gifs/Mentor.gif)

- Fazer login de usuário do tipo Mentor
  - Abrir e responder Avaliação
    - Fracassar na Avaliação
    - Conseguir ser aprovado
  - Abrir configurações de usuário

!['Faze Cadastro na Plataforma'](https://github.com/fga-eps-mds/2020.1-Minacademy-Wiki/blob/102-testes-funcionais/docs/produto/testesFuncionais/gifs/Register.gif)

- Fazer cadastro na plataforma como Aprendiz
  - Escolher gênero masculino
    - Tentar fazer com dados errados
    - Tentar escolher tipo aprendiz
    - Escolher tipo Mentor
  - Escolher gênero feminino
    - Escolher tipo aprendiz
- Abrir um certificado por link público
