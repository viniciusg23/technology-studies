# Test-Driven Development (TDD)
## Tipos de Erros em Softwares
Existes três tipos de erros na programação sendo eles: 
- Erros de sintaxe / compilação
- Erros em tempo de execução
- Erros semânticos ou de lógica
### Erros de sintaxe / compilação:
Erros que violam as normas gramaticais da linguagem e que são previamente identificador pela IDE e impedem que o código seja compilado.
### Erros em tempo de execução:
Não podem ser capturados pela IDE ou compilador já que são gerados em tempo de execução.
Ex: Divisão com denominador zero (a IDE não irá perceber isso antes da execução do código).
### Erros semânticos ou de lógica
São os erros mais difíceis de se detectar já que o código estará funcionando mas a saída estará incorreta de acordo com a proposta inicial do programa.
- - -
## Princípio de Teste de Software
O objeto de um teste dentro de um software é responder se o sistema foi construído corretamente e determinar se foi construído o sistema certo (de acordo com a proposta inicial do programa).
- - -
## Teste unitário
> Eles envolvem a verificação de pequenas unidades isoladas de código, como funções ou métodos, para garantir que eles funcionem conforme o esperado.

- O código do teste unitário chama o código operacional a partir de sua interface pública, de diversas maneiras e verifica os resultados.
- O teste não precisa ser exaustivo já que ele em si já agrega grande valor.

### Tipos de Teste Unitários
- **Básico:** Entradas simples é óbvias que devem funcionar (são sempre os primeiros testes a serem feitos)
- **Avançado:** Testes mais complexos quando o conhecimento do problema já é maior e nos leva a identificar potências casos estranhos de erros.
- **Fronteira:** Casos simples mas que representam condições extremas como: String vazia, null point, tipos diferentes, listas vazias, etc.

### Under testing x Over testing
Em um sistema não se deve testar literalmente cada elemento, já que isso irá causar um custo muito alto de testes durante o desenvolvimento do software, assim como, não se deve fazer poucos testes já que os erros que passarão despercebidos irão causar um custo muito alto no futuro de projeto para serem solucionados.

![](./image1.png)
- - -
## Teste-driven Development (TDD)
Teste Driven Development é uma técnica utilizada para desenvolvimento de software a partir de testes unitários feito antes da implementação de uma novo componente. 
### Como funciona:
1. Crie um novo teste;
2. Implementação mínima em seu novo componente para o teste falhar;
3. Implementação mínima do novo componente para o teste ter sucesso;
   - Deve ser implementado apenas o necessário para passar no teste, sem funcionalidades adicionais que não serão testadas.
4. Implementação final do novo componente (limpe o código);
5. Reexecute o teste para garantir que nada foi quebrado;

**Repita o processo…**
- - -
## Bibliotecas e F	rameworks de Testes
### Java
- [JUnit 5](https://junit.org/junit5/docs/current/user-guide/)
### Javascript / Typescript
- [Jest](https://jestjs.io/docs/getting-started)
- [Vitest](https://vitest.dev/guide/)
### Python
- [unittest](https://docs.python.org/3/library/unittest.html)
- [Pytest](https://docs.pytest.org/en/7.1.x/getting-started.html)