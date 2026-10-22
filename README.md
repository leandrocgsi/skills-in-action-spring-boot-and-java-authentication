# skills-in-action-spring-boot-and-java-authentication
### Base de código do projeto REST de pessoas e livros, em Spring Boot 4.1 e Java 25, usada como ponto de partida para adicionar autenticação com o Claude Code.

![Forks](https://img.shields.io/github/forks/leandrocgsi/skills-in-action-spring-boot-and-java-authentication)
![Stars](https://img.shields.io/github/stars/leandrocgsi/skills-in-action-spring-boot-and-java-authentication)
[![Donate with PayPal](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=ZJ4NQJXEKQ63A)

![Formação Spring Boot 2026](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/07-rest-java.png)

Este repositório é derivado do código do curso [Formação Spring Boot 2026: do Zero ao Deploy na AWS e GCP com Java, Docker e Kubernetes](https://pub.erudio.com.br/formacao-spring-boot-2026-do-zero-ao-continuous-deployment-na-aws-e-gcp-com-java-docker-e-kubernetes?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth), mas não é o código do curso. Ele foi atualizado para as versões mais recentes do framework e da linguagem e serve de base para o conteúdo da série *skills in action*.

# Cursos Relacionados

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/01-hm-claude-code-java.png "Formação Claude Code para DEVs Java e Spring Boot: Produtividade 10x, Agentes de IA, MCPs e Aplicações do Mundo Real")](https://pub.erudio.com.br/formacao-dev10x-claude-code-para-devs-java-e-spring-boot?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/14-microservices-java.png "Formação Microsserviços 2026: do Zero ao Deploy na Google Cloud com Spring Boot, Kubernetes e Docker")](https://pub.erudio.com.br/formacao-microsservicos-2026-do-zero-ao-deploy-na-google-cloud-com-spring-boot-kubernetes-e-docker?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/31-spring-ai-java.png "Formação Spring AI 2026: Inteligência Artificial com Java, Spring Boot, ChatGPT, DeepSeek, Claude e MCP")](https://pub.erudio.com.br/formacao-spring-ai-2026-inteligencia-artificial-com-java-spring-boot-chatgpt-deepseek-claude-e-mcp?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/10-docker-to-aws.png "Formação Docker e Kubernetes 2026: do Zero ao Deploy Profissional na AWS, Azure e GCP com GitHub Actions")](https://pub.erudio.com.br/docker-e-kubernetes-2026-do-zero-ao-deploy-profissional-na-aws-azure-e-gcp-com-github-actions?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/09-docker.png "Formação Docker e Kubernetes 2026: do Zero à Inteligência Artificial com MCP Catalog e Docker Model Runner")](https://pub.erudio.com.br/formacao-docker-kubernetes-do-zero-a-inteligencia-artificial-com-mcp?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/24-tests-java.png "Formação Java Testing 2026: Testes Automatizados com JUnit, Mockito, Spring Boot, TDD e TestContainers")](https://pub.erudio.com.br/formacao-java-testing-2026-testes-automatizados-com-junit-mockito-spring-boot-tdd-e-testcontainers?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/29-cdpl-java-gcp.png "Formação Continuous Deployment: do Zero ao Deploy com Java, Spring Boot, Docker, Kubernetes, Google Cloud (GCP) e GitHub Actions")](https://pub.erudio.com.br/formacao-continuous-deployment-java-kubernetes-gcp-github-actions?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/27-cicd-java-aws.png "Formação Continuous Integration e Delivery: do Zero ao Deploy com Java, Spring Boot, Docker, Amazon AWS e GitHub Actions")](https://pub.erudio.com.br/formacao-continuous-integration-delivery-java-aws-github-actions?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/28-cicd-java-azure.png "Formação Continuous Integration e Delivery: do Zero ao Deploy com Java, Spring Boot, Docker, Microsoft Azure e GitHub Actions")](https://pub.erudio.com.br/formacao-continuous-integration-delivery-java-azure-github-actions?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/13-career.png "Carreira em TI do Zero ao Exterior: Currículo, Entrevistas, Negociação e Crescimento Profissional")](https://pub.erudio.com.br/carreira-em-ti-do-zero-ao-exterior-curriculo-entrevistas-negociacao-e-crescimento-profissional?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

# Sobre este repositório

Este repositório é o ponto de partida de uma série de vídeos *skills in action*, em que o **Claude Code** e **skills** são usados para adicionar **autenticação com JWT** a uma API REST já existente. A base é uma API de pessoas e livros atualizada para **Spring Boot 4.1.1** e **Java 25**, ainda sem a camada de segurança.

## O que tem aqui hoje (ponto de partida)

* CRUD de pessoas e livros com paginação, ordenação e links HATEOAS
* Negociação de conteúdo em JSON, XML e YAML pelo header `Accept`
* Upload e download de arquivos, importação e exportação em CSV, XLSX e PDF (JasperReports), envio de e-mail e geração de QR Code
* Documentação da API com springdoc OpenAPI (Swagger UI)
* Migrations do banco com Flyway e MySQL
* Testes unitários, de repositório e de integração com Testcontainers, em JSON, XML e YAML

## Resultado final dos vídeos

Ao final da gravação o código deve ficar equivalente ao módulo `26_ShieldingOurAPIWithTests` do curso, já nas versões mais recentes das tecnologias:

* Spring Security com autenticação stateless via **JWT** (access token e refresh token)
* Endpoints `/auth/signin`, `/auth/refresh/{username}` e `/auth/createUser`
* Todos os endpoints `/api/**` protegidos, com Swagger UI e documentação liberados
* Usuários e permissões persistidos no banco com migrations Flyway
* Testes de integração que autenticam antes de chamar a API, em JSON, XML e YAML

## Como usar o código

### Pré-requisitos

* Java 25
* Maven 3.9+
* MySQL rodando em `localhost:3306` com usuário `root` e senha `admin123` (ajuste em `src/main/resources/application.yml` se for diferente)
* Docker em execução, necessário apenas para os testes que usam Testcontainers

### Passo a passo

1. Crie o banco de dados: `CREATE DATABASE rest_with_spring_boot_erudio;`
2. Execute a aplicação: `mvn spring-boot:run`. As migrations do Flyway criam e populam as tabelas na primeira execução
3. Acesse a documentação em `http://localhost:8080/swagger-ui/index.html`
4. Chame os endpoints em `/api/person/v1`, `/api/book/v1`, `/api/file/v1` e `/api/email/v1`
5. Rode a suíte de testes com `mvn test`
6. Abra o repositório no Claude Code e siga os vídeos para adicionar a autenticação

Para enviar e-mails defina as variáveis de ambiente `EMAIL_USERNAME` e `EMAIL_PASSWORD`. Os uploads são gravados no diretório configurado em `file.upload-dir`.

# Outros Cursos Erudio

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/01-rest-asp-net.png "Formação ASP.NET 2026: do Zero ao Deploy na Azure e GCP com .NET 10, Docker e Kubernetes")](https://pub.erudio.com.br/asp-net-2026-do-0-a-azure-e-gcp-com-asp-net-10-docker-e-kubernetes?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/33-dotnet-ai.png "Inteligência Artificial com .NET AI e .NET 10: Aplicações Inteligentes com ChatGPT, OpenAI, DeepSeek e Ollama")](https://pub.erudio.com.br/inteligencia-artificial-com-dotnet-ai-e-dotnet-10-apps-inteligentes-com-chatgpt-openai-deepseek-e-ollama?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/15-microservices-asp-net.png "Formação Microsserviços 2026: do 0 ao Deploy na Google Cloud com ASP.NET, .NET 10, Kubernetes e Docker")](https://pub.erudio.com.br/meus-cursos?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/32-code-ai-kspring.png "Formação Spring AI 2026: Inteligência Artificial com Kotlin, Spring Boot, ChatGPT, DeepSeek, Claude e MCP")](https://pub.erudio.com.br/formacao-spring-ai-2026-inteligencia-artificial-com-kotlin-spring-boot-chatgpt-deepseek-claude-e-mcp?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/22-ms-kotlin.png "Formação Microsserviços com Spring Cloud, Spring Boot, Kotlin, Docker e Zookeeper")](https://pub.erudio.com.br/formacao-microsservicos-com-spring-cloud-spring-boot-kotlin-docker-e-zookeeper?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/18-rest-spring-kotlin.png "Formação Spring Boot com Kotlin: REST APIs Profissionais do Zero ao Deploy na AWS com Docker e Kubernetes")](https://pub.erudio.com.br/formacao-spring-boot-com-kotlin-rest-apis-profissionais-do-zero-ao-deploy-na-aws-com-docker-e-kubernetes?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/20-kotlin.png "Kotlin para DEV's Java: Domine Lambdas, Generics, Reflections, Programação Funcional e Spring Boot")](https://pub.erudio.com.br/kotlin-para-desenvolvedores-java-domine-sintaxe-lambdas-generics-reflections-programacao-funcional-e-spring-boot?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

[![Image](https://raw.githubusercontent.com/leandrocgsi/blog-images/refs/heads/main/formacoes_github/30-jasper.png "Crie Relatórios Profissionais com JasperReports, Java, Spring Boot e JasperSoft Studio")](https://pub.erudio.com.br/crie-relatorios-profissionais-com-jasperreports-java-spring-boot-e-jaspersoft-studio?utm_source=github&utm_medium=organic&utm_campaign=readme&utm_content=sia-auth)

# Prévia Gratuita da versão anterior do curso

[![Prévia Gratuita](https://img.youtube.com/vi/fQAOaMqu0ho/maxresdefault.jpg)](https://www.youtube.com/watch?v=fQAOaMqu0ho)

## [Como Configurar Ambiente de DEV Spring Boot no Windows: Java, Maven, IntelliJ e MySQL Guia Completo](https://www.youtube.com/watch?v=M-0HxNoUeNE)

[![Montando um Ambiente de Desenvolvimento Spring Boot e Java no Windows: Minicurso Gratuito Completo!](https://img.youtube.com/vi/M-0HxNoUeNE/maxresdefault.jpg)](https://www.youtube.com/watch?v=M-0HxNoUeNE)

## [Como Configurar Ambiente de DEV Spring Boot no Linux: Java, Maven, IntelliJ e MySQL Guia Completo](https://www.youtube.com/watch?v=Wk5645fHrVU)

[![Montando um Ambiente de Desenvolvimento Spring Boot e Java no Linux: Minicurso Gratuito Completo!](https://img.youtube.com/vi/Wk5645fHrVU/maxresdefault.jpg)](https://www.youtube.com/watch?v=Wk5645fHrVU)

# Sobre REST

* [Web Services](http://www.semeru.com.br/blog/web-services/)
* [RESTful Web Services](http://www.semeru.com.br/blog/restful-web-services/)
* [HTTP Status Codes](http://www.semeru.com.br/blog/http-status-codes-em-servicos-rest/)
* [Do zero ao REST em 5 minutos com SpringBoot](http://www.semeru.com.br/blog/do-zero-ao-rest-em-5-minutos-com-springboot/)
* [Criando o primeiro endpoint REST com SpringBoot](http://www.semeru.com.br/blog/criando-o-primeiro-endpoint-rest-com-springboot/)
* [Documentando aplicações REST com SpringBoot e Swagger](http://www.semeru.com.br/blog/documentando-aplicacoes-restfull-com-springboot-e-swagger/)
* [Entendendo HATEOAS](http://www.semeru.com.br/blog/entendendo_hateoas/)
* [Aplicações RESTful HATEOAS com SpringBoot](http://www.semeru.com.br/blog/aplicacoes-restfull-hateoas-com-springboot/)

# HTTP Status Codes adotados pelas API's mais famosas do mundo

Essa lista se baseia [nesse repositório aqui!](https://gist.github.com/vkostyukov/32c84c0c01789425c29a#file-statuses-md)

|API                   | Status Codes                                                                             |
|----------------------|------------------------------------------------------------------------------------------|
|[Twitter][tw]         | 200, 304, 400, 401, 403, 404, 406, 410, 420, 422, 429, 500, 502, 503, 504                |
|[Stripe][stripe]      | 200, 400, 401, 402, 404, 429, 500, 502, 503, 504                                         |
|[Github][gh]          | 200, 400, 422, 301, 302, 304, 307, 401, 403                                              |
|[Pagerduty][pd]       | 200, 201, 204, 400, 401, 403, 404, 408, 500                                              |
|[NewRelic Plugins][nr]| 200, 400, 403, 404, 405, 413, 500, 502, 503, 503                                         |
|[Etsy][etsy]          | 200, 201, 400, 403, 404, 500, 503                                                        |
|[Dropbox][db]         | 200, 400, 401, 403, 404, 405, 429, 503, 507                                              |
|[Spotify][spf]        | 200, 201, 204, 304, 400, 401, 403, 404, 429, 500, 502, 503                               |
|[Google Cloud][gc]    | 200, 301, 304, 307, 308, 400, 401, 403, 404, 405, 409, 411, 412, 416, 429, 500, 501, 503 |
|[HipChat][hc]         | 200, 201, 202, 400, 401, 403, 404, 405, 429, 500, 503                                    |
|[Telegram][tg]        | 200, 303, 400, 401, 403, 404, 420, 500                                                   |
|[Pocket][pk]          | 200, 400, 401, 403, 503                                                                  |
|[Uber][ub]            | 200, 201, 400, 401, 403, 404, 406, 409, 422, 429, 500                                    |

Status codes **usados pela maioria deles**: 200, 201, 202, 204, 301, 302, 303, 304, 307, 308, 400, 401, 402, 403, 404, 405, 406, 408, 409, 410, 411, 412, 413, 416, 420, 422, 429, 500, 501, 502, 503, 504, 507

Usado por pelo menos **dois deles**: 200, 201, 204, 301, 304, 307, 400, 401, 403, 404, 405, 406, 409, 420, 422, 429, 500, 502, 503, 504

Usado por pelo menos **três deles**: 200, 201, 304, 400, 401, 403, 404, 405, 422, 429, 500, 502, 503

Usado por pelo menos **quatro deles**: 200, 201, 304, 400, 401, 403, 404, 405, 429, 500, 502, 503

Usado por pelo menos **cinco deles**: 200, 201, 400, 401, 403, 404, 405, 429, 500, 503

Usado por **todos eles**: 200, 400

[tw]: https://dev.twitter.com/overview/api/response-codes
[stripe]: https://stripe.com/docs/api#errors
[gh]: https://developer.github.com/v3/#client-errors
[pd]: https://developer.pagerduty.com/documentation/rest/errors
[nr]: https://docs.newrelic.com/docs/plugins/plugin-developer-resources/developer-reference/plugin-api-responses-error-codes
[etsy]: https://www.etsy.com/developers/documentation/getting_started/api_basics#section_standard_response_codes
[db]: https://www.dropbox.com/developers-v1/core/docs
[spf]: https://developer.spotify.com/web-api/user-guide/
[gc]: https://cloud.google.com/storage/docs/json_api/v1/status-codes#http-status-and-error-codes
[hc]: https://www.hipchat.com/docs/apiv2/response_codes
[tg]: https://core.telegram.org/api/errors
[pk]: https://getpocket.com/developer/docs/errors
[ub]: https://developer.uber.com/v1/api-reference/
