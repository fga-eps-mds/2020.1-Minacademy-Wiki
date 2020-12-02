## Introdução

O qualidade do software será verificada tanto por análises manuais como automáticas.

- Análises manuais: análises feitas pela gerência nos PRs para checagem de critérios da issue e de qualidade, além de verificação de atendimento às métricas. Além da verificação de alguns parâmetros definidos mais abaixo, a gerência também faz uma análise mais subjetiva de experiência de usuário para garantir que o PR entrega features com qualidades básicas de usabilidade. 
- Análises automáticas: testes unitários rodados pelo GitHub Actions e parâmetros de qualidade fornecidos pelo CodeClimate.

## Parâmetros

Para garantir a qualidade de software, os seguintes parâmetros foram definidos:

Métrica | Valores | Parâmetro mínimo | Momento da Validação | Método 
--------|---------|--------------|---------------|---------------
Manutenibilidade | A,B,C,D,E,F| B | Release 2 | CodeClimate
Cobertura de testes FrontEnd | 0-100%|30% | Pull Request | Jest Coverage e CodeClimate 
Cobertura de testes BackEnd | 0-100%| 90% | Pull Request | Jest Coverage e CodeClimate 
Critérios da issue atendidos | 0-100% | 100% | Pull Request | Manual

<small>*Parâmetros de PR exigidos a partir da sprint 8 </small>


## Medidas Preventivas

Algumas ferramentas e/ou padrões foram adotados em desenvolvimento para garantir a qualidade de código antes mesmo da revisão no PR. São elas:

- Ferramenta ESLint 
- Style guide do Airbnb
- Ferramenta Prettier para algumas correções automáticas

