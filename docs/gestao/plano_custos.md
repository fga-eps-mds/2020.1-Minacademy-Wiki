# Plano de Gerenciamento de Custos

| Data       | Versão | Descrição       | Autor              |
| ----       | ------ | ---------       | -----              |
| 03/09/2020 | 1.0    | Primeira Versão | Gabriela e Geovana |

## Estimativa de Horas

Para estimar as horas logo no início do projeto, iremos utilizar como base as 3 primeiras sprints. Na tabela abaixo, temos a média de horas trabalhadas por membro da equipe:


|   Sprint                                                  |         Média de horas por membro                                |
| ----------------------------------------------------------------- | --------------------------------------- |
| 1 | 4.375h |
| 2 | 6.875h |
| 3 | 6.75h |

Entretanto, a primeira sprint foi apenas documentação e ambientação para MDS. A partir da segunda, o ritmo do projeto começou a entrar no ritmo que será empregado até que o produto esteja pronto. Considerando a entrada de mais entregas de código nas sprints seguintes, vamos estimar uma média de horas semanais por membro de **8h**.

Considerando que temos 15 sprints de 7 dias até a entrega do produto (a Release 2 será na 16º sprint), então temos:

> 8h * 15 semanas = **120h** por membro

E para o projeto como um todo:

> 120h * 8 membros = **960h** de projeto

## Perfil Profissional

A seguir podemos ver o perfil da equipe em relação ao mercado de trabalho.

| Função         | Tempo de experiência na área | Nível                             | Carga Horária | Quantidade de Profissionais
| :---           | :----                        | :---                              | :---          | :---
| Desenvolvedor  | ~ 1 ano                      | Ensino Médio Completo (graduando) | 20h           | 6
| Product Owner  | Nenhuma                      | Ensino Médio Completo (graduando) | 20h           | 1
| Scrum Master   | Nenhuma                      | Ensino Médio Completo (graduando) | 20h           | 1

## Estimativa de Custo

Os valores abaixo foram baseados nos dados fornecidos pelo site [Vagas.com](vagas.com).

Para o custo, vamos considerar os salários médios a seguir:

Cargo de Referência             | Salário Mensal Médio | Função no Projeto | Referência                                                                  |
:---                            | :---                 | :---              | :---                                                                        |
Estagiário em Desenvolvimento   | R$ 1.133, 00          | Desenvolvedor     | [Link](https://www.vagas.com.br/cargo/estagiario-desenvolvedor)             |
Estágio em Gerenciamento        | R$ 1.757,00           | Gerente           | [Link](https://www.vagas.com.br/cargo/estagio-em-gerenciamento-de-projetos) |

Considerando o custo com equipamentos e infraestrutura, temos:

| Equipamento / Serviço | Valor                  | Medida    | Referência
| :---                  | :---                   | :---      | :--- |
| Internet              | R$ 119,99              | R$/mês    | [Link](https://internet.vivo.com.br/vivo-fibra/banda-larga/oferta/?gclid=Cj0KCQjwtZH7BRDzARIsAGjbK2ZIFI-ttd73jQrcZV6-FS4G9fay8hgXQJD9c4aypZ6Zgym-Crhq5CsaAi5ZEALw_wcB&gclsrc=aw.ds) |
| Computador            | R$ 3.514,05             | Unitário  | [Link](https://www.magazineluiza.com.br/notebook-lenovo-ultrafino-ideapad-s145-i5-1035g1-8gb-256gb-ssd-windows-10-15-6-82dj0003br-prata/p/ab82k6ejha/in/note/?&seller_id=lenovo&&utm_source=google&utm_medium=pla&utm_campaign=&partner_id=57204&gclid=Cj0KCQjwtZH7BRDzARIsAGjbK2aaGcYU5ANhv_Su6MjH2b9BWjp4GcnX061TPw7USQh7_U_m0DOSQ3YaApnpEALw_wcB)
| \*Energia               | R$ 0,82                | R$/Hora   | [Link](http://simuladortarifabranca.ceb.com.br/public/index/step-resultado/perfil/2)

\* _Foi considerado o consumo de uma fonte de notebook 65W e um roteador de 12W_

Considerando esses dados, vamos calcular os custos homem/hora e considerando todo o tempo do projeto:

### Desenvolvedores - salário
> 1.133,00 R$ / 20h = **56,65 R$/h**

### Gerentes - salário
> 1.757,00 R$ / 20h =  **87,85 R$/h**

### Internet
> 119,00 R$ / 80h (4 semanas, equivalente à 1 mês) = **1,49 R$/h**

### Energia
> **0,82 R$/h**

### Computador
> 3.514,05 R$ / 120 (horas de projeto) = **R$ 29,28**

Logo, para o projeto como um todo temos:

### Soma dos valores:
Desenvolvedores
> 56,65 + 1,49 + 0,82 + 29,28 = **R$ 88,24**

Gerentes
> 87.85 + 1,49 + 0,82 + 29,28 = **R$ 119,44**

<!-- > 55 R$/h * 960h = **52.800** -->
| Homem / hora - Gerentes (2)    | Homem / hora - Desenvolvedores (6) | Total         |
| :--                            | :--                                | :--           |
| R$ 119,44                      | R$ 88,24                           | 92.198,4      |