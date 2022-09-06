## Domain-Driven Design:

Desenvolvimento orientado ao domínio é excelente para modelar regras de negócio complexas mas não faz tanto sentido em situações mais simples.

### Domínio:

O **domínio** é o problema que uma organização precisa resolver para poder implementar um software que realmente atende as necessidades do negócio dos seus clientes.

A seguir, exemplos de algumas empresas com seus respectivos domínios:

- SAP: Auxilia na gestão financeira, de produção, suprementos, RH, contábil das empresas;
- HubSpot: Ajuda na prospecção, captação e conversão de leads em vendas;
- Salesforce: Cuida de todo o ciclo de relacionamento até o fechamento das vendas;
- Vimeo: Realiza streaming de vídeo;

### Linguagem ubiqua:

[![UbiquitousLanguage](https://raw.githubusercontent.com/victorreinor/clean-code-clean-architecture-course/master/class-04/images/ubiquitous-language.png "UbiquitousLanguage")](https://raw.githubusercontent.com/victorreinor/clean-code-clean-architecture-course/master/class-04/images/ubiquitous-language.png "UbiquitousLanguage")

A linguagem ubiqua é falada entre os especilistas no domínio e a equipe de desenvolvimento dentro de um determinado contexto delimitado, que é local onde aquele domínio se aplica.
Além disso, a linguagem ubiqua deve ser refletida dentro do código-fonte, não apenas em documentos, diagramas e glossários.

#### Bounded context:

Um **bounded context** é onde o problema é resolvido, está no espaço da solução, forma um limite explícito dentro do qual um modelo de domínio será implementado.

A forma de interação entre cada bounded conotext é detalhada em um **context map**

### Tipos de subdominio

- Core ou basic: É o mais importante e que traz amis valor para empresa, é onde você coloca seus amiores e melhores esforços;
- Support ou Auxiliary: Complementa o core domain, sem ele não é possível ter sucesso no negócio;
- Generic: É um subdomínio que pode ser delegado para outra empresa ou mesmo ser um produto de mercado;

---

Problema = Sub domínio
Solução = Bounded Context