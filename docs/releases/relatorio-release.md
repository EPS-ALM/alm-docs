# Relatório de Release - Release 1.0.0

Este relatório avalia, seguindo os critérios de avaliação propostos pelo professor, a primeira release do projeto de ALM.

## Critérios de Avaliação Coletiva

### 1. Práticas Ágeis

#### a. Commits atômicos

Executando o comando `git log --pretty=format:"%h - %an, %ar : %s" -n 10` é possível visualizar os últimos 10 commits do repositório. A partir disso, é possível observar que os commits são atômicos:

<details>
  <summary>alm-docs</summary>
  <img src="../assets/commits-alm-docs.png" alt="Commits do repositório alm-docs">
</details>

<details>
  <summary>alm-liability</summary>
  <img src="../assets/commits-alm-liability.png" alt="Commits do repositório alm-liability">
</details>

<details>
  <summary>alm-frontend</summary>
    <img src="../assets/commits-alm-frontend.png" alt="Commits do repositório alm-frontend">
</details>

<details>
  <summary>alm-assets</summary>
    <img src="../assets/commits-alm-assets.png" alt="Commits do repositório alm-assets">
</details>

<details>
  <summary>alm-service</summary>
    <img src="../assets/commits-alm-service.png" alt="Commits do repositório alm-service">
</details>

<details>
  <summary>alm-risk-manager</summary>
    <img src="../assets/commits-alm-risk-manager.png" alt="Commits do repositório alm-risk-manager">
</details>

<details>
  <summary>stocks-forecasting</summary>
    <img src="../assets/commits-stocks-forecasting.png" alt="Commits do repositório stocks-forecasting">
</details>

#### b. Documentação das sprints

A documentação das sprints está disponível no repositório `alm-docs`. A documentação da primeira sprint pode ser acessada [aqui](../artefatos/relatorio-semanal.md).

#### c. Quantidade de Issues

Devido ao caráter avaliativo da disciplina, as issues foram centralizadas no repositório `alm-docs`. A quantidade de issues pode ser visualizada [aqui](https://github.com/EPS-ALM/alm-docs/issues).

##### Média de Issues

Considerando que, nesse momento, existem 54 issues cadastradas. A média de issues por sprint é de, aproximadamente, 7.

![Média de Issues por Sprint](./assets/issues.png)

#### d. Pull Requests

A quantidade de pull requests para cada repositório pode ser visualizada abaixo:

<details>
  <summary>alm-docs</summary>
  <img src="../assets/pr-alm-docs.png" alt="Pull Requests do repositório alm-docs">
</details>

<details>
  <summary>alm-liability</summary>
  <img src="../assets/pr-alm-liability.png" alt="Pull Requests do repositório alm-liability">
</details>

<details>
  <summary>alm-frontend</summary>
    Não houve necessidade de Pull Requests pois o desenolvimento foi feito por um único membro.
</details>

<details>
  <summary>alm-assets</summary>
    <img src="../assets/pr-alm-assets.png" alt="Pull Requests do repositório alm-assets">
</details>

<details>
  <summary>alm-service</summary>
    <img src="../assets/pr-alm-service.png" alt="Pull Requests do repositório alm-service">
</details>

<details>
  <summary>alm-risk-manager</summary>
    <img src="../assets/pr-alm-risk-manager.png" alt="Pull Requests do repositório alm-risk-manager">
</details>

<details>
  <summary>stocks-forecasting</summary>
  Não houve necessidade de Pull Requests pois o desenolvimento foi feito em pareamento síncrono.
</details>

#### e. Qualidade das Issues

As issues estão bem descritas e organizadas. A descrição das issues é clara e objetiva, facilitando a compreensão do que deve ser feito. Porém, a análise deve ser comprovada manualmente para cada repositório.

#### f. Qualidade dos Pull Requests

Os pull requests não possuem documentação, checkilist, ou qualquer outra forma de garantir a qualidade do código além da revisão manual. A análise de qualidade deve ser comprovada manualmente para cada repositório.

#### g. Velocity e curva de commits

A curva de commits pode ser obtida atráves do comando `•git log --pretty=format:"%ad" --date=short | sort | uniq -c`. A curva de commits para cada repositório pode ser visualizada abaixo:

<details>
  <summary>alm-docs</summary>
  <img src="../assets/velocity-alm-docs.png" alt="Commits do repositório alm-docs">
  <img src="../assets/velocity-github-alm-docs.png" alt="Commits do repositório alm-docs no github">
</details>

<details>
  <summary>alm-liability</summary>
  <img src="../assets/velocity-alm-liability.png" alt="Commits do repositório alm-liability">
  <img src="../assets/velocity-github-alm-liability.png" alt="Commits do repositório alm-liability no github">
</details>

<details>
  <summary>alm-frontend</summary>
    <img src="../assets/velocity-alm-frontend.png" alt="Commits do repositório alm-frontend">
    <img src="../assets/velocity-github-alm-frontend.png" alt="Commits do repositório alm-frontend no github">
</details>

<details>
  <summary>alm-assets</summary>
    <img src="../assets/velocity-alm-assets.png" alt="Commits do repositório alm-assets">
    <img src="../assets/velocity-github-alm-assets.png" alt="Commits do repositório alm-assets no github">
</details>

<details>
  <summary>alm-service</summary>
    <img src="../assets/velocity-alm-service.png" alt="Commits do repositório alm-service">
    <img src="../assets/velocity-github-alm-service.png" alt="Commits do repositório alm-service no github">
</details>

<details>
  <summary>alm-risk-manager</summary>
    <img src="../assets/velocity-alm-risk-manager.png" alt="Commits do repositório alm-risk-manager">
    <img src="../assets/velocity-github-alm-risk-manager.png" alt="Commits do repositório alm-risk-manager no github">
</details>

<details>
  <summary>stocks-forecasting</summary>
    <img src="../assets/velocity-stocks-forecasting.png" alt="Commits do repositório stocks-forecasting">
    <img src="../assets/velocity-github-stocks-forecasting.png" alt="Commits do repositório stocks-forecasting no github">
</details>

### 2. Práticas DevOps

Deploy automático do repositórios de alm-liability, alm-assets, alm-service e alm-risk-manager foi realizado no Heroku:

- **Service**: [alm-service](https://alm-service-eae21cd8fb32.herokuapp.com/portfolio-allocation)
- **Assets**: [alm-assets](https://alm-assets-898cc81ff044.herokuapp.com/)
- **Risk Manager**: [alm-risk-manager](https://almriskmanager-16e9ecd81666.herokuapp.com/)
- **Liability**: [alm-liability](http://187.84.176.16:10100/docs)

Já o repositório alm-docs foi hospedado no GitHub Pages:

- **Docs**: [alm-docs](https://eps-alm.github.io/alm-docs/) - [workflow](https://github.com/EPS-ALM/alm-docs/blob/main/.github/workflows/main.yml)

Por fim, o repositório do frontend foi hospedado no OnReader:

- **Frontend**: [alm-frontend](https://alm-frontend.onrender.com/)

### 3. Escopo e Arquitetura

- [Story Map](../artefatos/storymap/personas.md)
- [Protótipo](../artefatos/prototipo.md)
- [Arquitetura](../artefatos/arquitetura.md)

## Critérios de Avaliação Individual

### 1. Quantidade total de commits

A quantidade total de commits para cada repositório e cada integrante pode ser visualizada abaixo:

<details>
  <summary>alm-docs</summary>
  <img src="../assets/commits-alm-docs-individual.png" alt="Commits do repositório alm-docs por integrante">
</details>

<details>
  <summary>alm-liability</summary>
  <img src="../assets/commits-alm-liability-individual.png" alt="Commits do repositório alm-liability por integrante">
</details>

<details>
  <summary>alm-frontend</summary>
    <img src="../assets/commits-alm-frontend-individual.png" alt="Commits do repositório alm-frontend por integrante">
</details>

<details>
  <summary>alm-assets</summary>
    <img src="../assets/commits-alm-assets-individual.png" alt="Commits do repositório alm-assets por integrante">
</details>

<details>
  <summary>alm-service</summary>
    <img src="../assets/commits-alm-service-individual.png" alt="Commits do repositório alm-service por integrante">
</details>

<details>
  <summary>alm-risk-manager</summary>
    <img src="../assets/commits-alm-risk-manager-individual.png" alt="Commits do repositório alm-risk-manager por integrante">
</details>

<details>
  <summary>stocks-forecasting</summary>
    <img src="../assets/commits-stocks-forecasting-individual.png" alt="Commits do repositório stocks-forecasting por integrante">
</details>

### 2. Quantidade de Issues Alocadas

A quantidade de issues alocadas para cada integrante pode ser visualizada abaixo:

- [Arthur Ferreira Rodrigues](https://github.com/EPS-ALM/alm-docs/issues/assigned/ArthurFerreiraRodrigues)
- [Lucas Pimentel Quintão](https://github.com/EPS-ALM/alm-docs/issues/assigned/LucasPimentel123)
- [Augusto Durães Camargo](https://github.com/EPS-ALM/alm-docs/issues/assigned/augustocrmg)
- [Cristian Furtado](https://github.com/EPS-ALM/alm-docs/issues/assigned/csafurtado)
- [Deivid Carvalho](https://github.com/EPS-ALM/alm-docs/issues/assigned/deivid-a1)
- [Eduardo Maia Rezende](https://github.com/EPS-ALM/alm-docs/issues/assigned/eduardomr)
- [Eliás Yousef](https://github.com/EPS-ALM/alm-docs/issues/assigned/eliasyousef00)
- [Fernando Vargas](https://github.com/EPS-ALM/alm-docs/issues/assigned/SFernandoS)
- [Gustavo Barbosa](https://github.com/EPS-ALM/alm-docs/issues/assigned/brbsg)
- [Gustavo Martins Ribeiro](https://github.com/EPS-ALM/alm-docs/issues/assigned/gustavomartins-github)
- [José Luís Ramos Teixeira](https://github.com/EPS-ALM/alm-docs/issues/assigned/joseluis-rt)
- [Luis Guilherme](https://github.com/EPS-ALM/alm-docs/issues/assigned/luisgaboardi)
- [Marcos Vinícius de Deus](https://github.com/EPS-ALM/alm-docs/issues/assigned/Marcos574)
- [Pablo Christianno Silva Guedes](https://github.com/EPS-ALM/alm-docs/issues/assigned/PabloChristianno)
- [Pedro Vitor Augusto de Jesus](https://github.com/EPS-ALM/alm-docs/issues/assigned/Peedrooo)
- [Sávio Cunha](https://github.com/EPS-ALM/alm-docs/issues/assigned/savioc2)
- [Victor Hugo](https://github.com/EPS-ALM/alm-docs/issues/assigned/8ifq3)
- [Wesley Santos](https://github.com/EPS-ALM/alm-docs/issues/assigned/wesleysantos00)

## Critérios de Avaliação da Release 1 do MVP

### 1. Story Map

O story map foi desenvolvido e pode ser acessado [aqui](../artefatos/storymap/personas.md).

### 2. Épicos, features e US

As features planejadas podem ser visualizadas no [GitHub](https://github.com/EPS-ALM/alm-docs/labels/Feature).

### 3. Protótipo

O protótipo foi desenvolvido e pode ser acessado [aqui](../artefatos/prototipo.md).

### 4. Código - Implementação

Deve ser analisado manualmente para cada repositório:

- [alm-docs](https://gitub.com/EPS-ALM/alm-docs)
- [alm-risk-manager](https://github.com/EPS-ALM/alm-risk-manager)
- [alm-service](https://github.com/EPS-ALM/alm-service)
- [alm-assets](https://github.com/EPS-ALM/alm-assets)
- [alm-liability](https://github.com/EPS-ALM/alm-liability)
- [stocks-forecasting](https://github.com/EPS-ALM/stocks-forecasting)

### 5. Arquitetura Documentada

A arquitetura foi documentada e pode ser acessada [aqui](../artefatos/arquitetura.md).

### 6. Configuração do Ambiente

Prcessos de setup de ambiente podem ser acessados no README de cada repositório.

### 7. GitPages

O GitHub Pages foi configurado para o repositório `alm-docs` e pode ser acessado [aqui](https://eps-alm.github.io/alm-docs/).

### 8. Padrões Software Livre

Os padrões de software livre foram seguidos e podem ser acessados pelo GitHub:

- [ReadMe](https://github.com/EPS-ALM/alm-docs/blob/main/README.md)
- [Code of Conduct](https://github.com/EPS-ALM/alm-docs/blob/main/CODE_OF_CONDUCT.md)
- [Contributing](https://github.com/EPS-ALM/alm-docs/blob/main/CONTRIBUTING.md)

### 9. Release Notes

As releases não tiveram suas notas documentadas.

# Documento de Release Assinado

O documento de release foi assinado por todos os membros da equipe e pode ser acessado [aqui](./primeira-release-assinado.pdf).

# Alterações

Não devem ser realizadas alterações nessa página, visto que o documento deve permanecer idêntico ao assinado pelos membros da equipe.

Data de assinatura: 21/12/2024