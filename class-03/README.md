### Ports and Adapters:

Nasceu para resolver um problema das aplicações na década passada que era acumulo de regras de négocios na interface gráfica e no banco de dados, por conta desse acumulo não era possivel testar aplicação de forma automatizada.

[![PortsAndAdapters](https://raw.githubusercontent.com/victorreinor/clean-code-clean-architecture-course/master/class-03/images/portsandadapters.png "PortsAndAdapters")](https://raw.githubusercontent.com/victorreinor/clean-code-clean-architecture-course/master/class-03/images/portsandadapters.png "PortsAndAdapters")

#### Artigos:

- https://web.archive.org/web/20060625193207/http://alistair.cockburn.us/crystal/articles/hpaaa/hexagonalportsandadaptersarchitecture.htm
- https://jmgarridopaz.github.io/content/hexagonalarchitecture.html

### Clean Architecture:

A Clean Architecture é um modelo arquitetural orientada ao desacoplamento entre as regras de negócio, ou domínio, da aplicação e os recursos externos como frameworks e banco de dados.

O Bob Martin reforça que a ideia de clean architecture que o centro da aplicação não é o banco de dados, framework, lib e etc... E sim os **use cases**

[![CleanArchitecture](https://raw.githubusercontent.com/victorreinor/clean-code-clean-architecture-course/master/class-03/images/cleanarchitecture.png "CleanArchitecture")](https://raw.githubusercontent.com/victorreinor/clean-code-clean-architecture-course/master/class-03/images/cleanarchitecture.png "CleanArchitecture")

- **Entities:**
  - Regras de negócios independentes e que podemos aplicar de diversas formas.
- **Use Cases:**
  - Camada externa que orquestram o fluxo de dados para entidades (Entities).
- 

#### Artigos:

- https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html