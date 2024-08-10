# Desenvolvimento Orientado a Testes (TDD)

## Estrutura do Repositório

- `starter.go`: Arquivo principal que tem as funções que vão ser testadas.
- `starter_test.go`: Arquivo de teste com exemplos de TDD .
- `coverage.out` e `coverage.html`: Arquivos gerados para análise de cobertura de código.
- `README.md`: Este arquivo, contendo documentação do projeto.

## Rodando os Exemplos e Funções

Vou demonstrar como executar os exemplos de testes em Go, seguindo a abordagem de TDD.

Utilizei o comando "go test -v" para rodar todos os testes do arquivo starter_test.go. 


<img width="847" alt="image" src="https://github.com/user-attachments/assets/1ae109dc-b35c-45da-907f-cee39b82fcb3">



<img width="652" alt="image" src="https://github.com/user-attachments/assets/12499b7e-9e04-462b-a582-6199b2cc0971">


<img width="651" alt="image" src="https://github.com/user-attachments/assets/248e3836-bf61-4cdf-a92b-edb57373d3d7">



## Analisando a Cobertura de Códigos 

Para garantir a qualidade dos testes, gerei um relatório de cobertura de código com os comandos abaixo:

go test -v -coverprofile=coverage.out
go tool cover -html=coverage.out -o coverage.html


<img width="704" alt="image" src="https://github.com/user-attachments/assets/3d017118-9c29-46ec-b033-dcf7171dad8a">


Em seguida, abri o arquivo coverage.html no navegador para visualizar a cobertura de código de forma gráfica.


<img width="1265" alt="image" src="https://github.com/user-attachments/assets/d1408850-2126-4585-9268-255ec417f190">




## Técnicas e Conceitos de TDD

##### Red-Green-Refactor

###### 1. Red: Um teste é escrito inicialmente para falhar, já que a funcionalidade ainda não está implementada.
###### 2. Green: O código necessário é implementado para que o teste passe.
###### 3. Refactor: O código é refatorado para melhorar sua compreensão e manutenção, mantendo todos os testes com sucesso.

##### Testes Unitários

###### Testes unitários são escritos para garantir que cada função individual funcione corretamente. Isso permite a identificação e correção de erros de forma rápida e eficaz durante o desenvolvimento.

##### Testes de Integração

###### Testes de integração são desenvolvidos, especialmente para funções que dependem de múltiplos componentes, como a função `CheckHealth`. Esses testes garantem que os diferentes módulos do sistema funcionem em conjunto como esperado.


##### O Test-Driven Development é uma prática essencial no desenvolvimento de software, pois incentiva a criação de código limpo, modular e testável. Com o TDD, os desenvolvedores escrevem testes antes de implementar a funcionalidade, garantindo que cada parte do código atenda aos requisitos esperados desde o início. Isso reduz a probabilidade de bugs, facilita a refatoração e melhora a qualidade geral do software.
