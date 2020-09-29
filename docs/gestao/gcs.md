# Gerência de Configuração de Software

| Data       | Versão | Descrição       | Autor              |
| ----       | ------ | ---------       | -----              |
| 29/09/2020 | 1.0    | Primeira Versão | Gabriela           |

## Commits

Todos os commits devem possuir um título que demonstra resumidamente as alterações que foram feitas. Se o título não for suficiente para descrever as modificações, o commit também deve possuir uma descrição com a separação de uma linha do título.

```md
  Título do commit

  Descrições necessárias para a total compreensão das alterações
```

## Pull Requests

O padrão de PR's pode ser encontrado no arquivo `.github/PULL_REQUEST_TEMPLATE.md`. Nele é fornecido um padrão com as seguintes informações:

| Nome | Obrigatório | Opções |
| :--- | :--- | :--- |
| Título do PR | Sim | - |
| Issue Relacionada | Sim | - |
| Como isso foi testado? | Sim | Teste unitário ou Testes exploratório |
| Imagens | Não | - |
| Essa modificação exige atualização da documentação? | Sim | Sim ou Não |
| Tipo de alteração | Sim | Nova feature, Correção de bugs, Alteração de uma funcionalidade já existente ou Documentação

## Validação de Pull Requests

A aprovação de um PR está condicionada à aceitação dele por pelo menos um membro de EPS. Essa aceitação só será concedida caso os testes unitários passem, o código esteja rodando e de acordo com os padrões e arquitetura do projeto.

## Issues

O padrão de issue que é automaticamente carregado ao se criar uma issue no repositório pode ser acessado em `.github/ISSUE_TEMPLATE.md`. Esse padrão possui os seguintes campos de informações:

| Nome | Obrigatório |
| :--- | :--- |
| Nome da Issue | Sim |
| Descrição | Sim |
| Solução | Apenas para bugfix |
| Critérios de Aceitação | Não |

## Branches

### Features e Documentações

Todas as branches criadas, exceto para bugfix, devem possuir o formato ` numero_da_issue-nome-da-issue `

Exemplo:

`55-nome-reduzido`

### Bugfix

No caso de uma branch criada para a resolução de um bugfix, ela deve possuir o formato `bugfix-numero_da_issue-nome-da-issue`

Exemplo:

`bugfix-56-nome-reduzido`

### Política de Branches

Nesse projeto utilizamos o [GitFlow](https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow) conforme mostrado na imagem abaixo:
