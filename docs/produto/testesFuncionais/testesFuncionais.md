# Teste Funcional

O teste funcional visa verificar a aceitabilidade dos dados, do processamento, da resposta do mesmo e a implementação apropriada das regras de negócio. Esse teste visa verificar o sistema através da interação da Interface Gráfica de Usuário(GUI) e analisar as saídas e resultados dessa interação.
Para realizar o teste funcional foi utilizado o **Cypress**, um framework de testes automatizados end-to-end. Como os repositórios do backend e frontend são separados, não foi possível colocar na integração contínua(CI), porém é possível rodar localmente rodando o script “npm run cypress”. Os testes podem ser visualizados nos gif’s abaixo.

## Cobertura do Teste

- *01/12/2020*

!['Cobertura dos testes feita no dia 01/12/2020'](cobertura.png 'Feita no dia 01/12/2020')

## Testes executados no projeto

### Teste 1

!['Teste de Aprendiz'](gifs/Learner.gif)

- Fazer login com usuário não cadastrado
- Fazer login com usuário do tipo aprendiz
  - Acessar aba de certificados
  - Verificar certificados

### Teste 2

!['Teste de Mentor'](gifs/Mentorship.gif)

- Fazer login de usuário do tipo Mentor
  - Abrir e responder Avaliação
    - Fracassar na Avaliação
    - Conseguir ser aprovado
  - Abrir configurações de usuário

### Teste 3

!['Fazer Cadastro na Plataforma'](gifs/Register.gif)

- Fazer cadastro na plataforma como Aprendiz
  - Escolher gênero masculino
    - Tentar fazer com dados errados
    - Tentar escolher tipo aprendiz
    - Escolher tipo Mentor
  - Escolher gênero feminino
    - Escolher tipo aprendiz

### Teste 4

!['Abrir o chat da plataforma'](gifs/Chat.gif)

- Abrir um chat

### Teste 5

- Abrir um certificado por link público
