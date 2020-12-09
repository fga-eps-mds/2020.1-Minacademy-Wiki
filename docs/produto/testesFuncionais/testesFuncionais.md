# Teste Funcional

O teste funcional visa verificar a aceitabilidade dos dados, do processamento, da resposta do mesmo e a implementação apropriada das regras de negócio. Esse teste visa verificar o sistema através da interação da Interface Gráfica de Usuário(GUI) e analisar as saídas e resultados dessa interação.
Para realizar o teste funcional foi utilizado o **Cypress**, um framework de testes automatizados end-to-end. Como os repositórios do backend e frontend são separados, não foi possível colocar na integração contínua(CI), porém é possível rodar localmente rodando o script “npm run cypress”. Os testes podem ser visualizados nos gif’s abaixo.

## Cobertura do Teste

- *01/12/2020*

!['Cobertura dos testes feita no dia 01/12/2020'](cobertura.png 'Feita no dia 01/12/2020')

## Testes executados no projeto

### Teste do Login 

!['Teste do Login'](gifs/Login.gif)

- tentar fazer login com usuário não cadastrado
- Fazer login com usuário do tipo aprendiz

### Teste do Tutorial

!['Teste Tutorial'](gifs/Tutorial.gif)

- Acessar o tutorial
  - Abrir e responder a última atividade restante de forma incorreta
  - Responder a atividade corretamente


### Teste da Avaliação Para Se Tornar Mentor

!['Fazer Prova de Mentoria'](gifs/Exam.gif)

- Fazer avaliação para validar mentor
  - Fazer login com mentor
  - Falhar na primeira tentativa da avaliação
  - Passar na segunda tentativa da avaliação

### Teste da funcionalidade Mentoria

!['Teste Mentoria'](gifs/Mentorship.gif)

- Acessar a página de mentoria
    - Cancelar solicitação de mentor
    - Solicitar mentor
    - Clicar em desvincular
    - Clicar em cancelar
    - Clicar em desvincular novamente e confirmar fim do vínculo
    - Solicitar um novo mentor

### Teste do Cadastro

!['Fazer Cadastro na Plataforma'](gifs/Register.gif)

- Fazer cadastro na plataforma como Aprendiz
  - Tentar fazer com dados inválidos
    - Tentar escolher tipo aprendiz
    - Escolher tipo Mentor
  - Tentar fazer com dados válidos
    - Escolher gênero feminino
    - Escolher tipo aprendiz

### Teste do Chat

!['Abrir o chat da plataforma'](gifs/Chat.gif)

- Abrir um chat
- Mandar uma mensagem
### Teste da Pagina de Certificados

  !['Acessar os certificados'](gifs/CertificateAccess.gif)

  - Abrir um certificado por link público

### Teste do Acesso de um Certificado 

!['Abrir um certificado'](gifs/Certificate.gif)

- Abrir um certificado por link público

