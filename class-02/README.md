Este conteúdo foi feito na segunda aula do curso Clean Code e Clean Architecture da Branas.io

Nessa aula percorremos os assuntos **TDD** e **Test patterns**.

### TDD

Quando criamos um teste devemos seguir os conjuntos abaixo:

Para a descrição do teste utilizamos:

- Given: Definição de todas as informações necessárias para executar o comportamento que será testado;
- When: Executar o comportamento;
- Then: Verificar o que aconteceu após a execução, comparando as informações retornadas com a expectativa que foi criada

Para testar o comportamento:

- Arrange: Definição de todas as informações necessárias para executar o comportamento que será testado
- Act: Executar o comportamento
- Assert: Verificar o que aconteceu após a execução, comparando as informações retornadas com a expectativa que foi criada

Os testes devem seguir o padrão:

FIRST:

- Fast: Os testes devem rodar rápido;
- Independent: Não deve existir dependência entre os testes, eles devem poder ser executados de forma isoladas;
- Repeatable: O resultado deve ser o mesmo independente da quantidade de vezes que seja executado;
- Self-validating: O próprio teste deve ter uma saída bem definida que é válida ou não fazendo com que ele passe ou falhe;
- Timely: Os testes devem ser escritos antes do código-fonte;

### Test patterns:

- Dummy: Objetos que criamos apenas para completar a lista de parâmetros que precisamos passar para invocar um determinado método;
- Stubs: Objetos que retornam respostas prontas, definidas para um determinado teste, por questão de performance ou segurança (exemplo: quando eu executar o método fazer pedido preciso que o método pegar cotação do dólar retorne R$3,00);
- Spies: Objetos que "espionam" a execução do método e armazenam os resultados para verificação posterior (exemplo:  quando eu executar o método fazer pedido preciso saber se o método enviar email foi invocado internamente e com quais parâmetros);
- Mocks: Objetos similares a stubs e spies, permitem que você diga exatamente o que quer que ele faça e o teste vai quebrar se isso não acontecer
- Fake: Objetos que tem implementações que simulam o funcionamento da instância real, que seria utilizada em produção (exemplo: uma base de dados em memória)

**Para mais informações acesse**:

https://app.branas.io/clean-code-e-clean-architecture

Executar:

Instalar dependências:

`yarn install`

Rodar testes:

`npx jest --watchAll --coverage` || `npx jest com as opções --coverage`

Configurar o projeto do zero:

`yarn init -y`

`yarn add typescript jest @types/jest ts-node ts-jest`

`npx tsc --init`

`npx ts-jest config:init`