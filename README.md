# Sistema de Escalas

> Aplicação web para visualização e organização de jornadas, escalas e pausas, desenvolvida como parte do ecossistema de projetos do `eubruno-coder`.

[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-orange)](#status-do-projeto)
[![Versão](https://img.shields.io/badge/versão-V1-blue)](#roadmap)
[![Tecnologia](https://img.shields.io/badge/tecnologia-HTML%20%7C%20CSS%20%7C%20JavaScript-yellow)](#arquitetura)
[![Deploy](https://img.shields.io/badge/deploy-GitHub%20Pages-222?logo=github)](#deploy)
[![Licença](https://img.shields.io/badge/licença-a%20definir-lightgrey)](#licenciamento)

---

## Sobre o projeto

O **Sistema de Escalas** é uma aplicação web focada na organização visual da jornada de trabalho, permitindo acompanhar horários, pausas e eventos da escala de maneira simples e objetiva.

A V1 foi concebida como uma aplicação **front-end independente**, sem necessidade de servidor ou banco de dados para funcionamento básico. O objetivo é manter uma implantação simples e, ao mesmo tempo, criar uma base técnica que possa evoluir para persistência, autenticação e gestão centralizada.

O projeto também faz parte do ecossistema de soluções desenvolvido pelo `eubruno-coder`, mantendo integração conceitual e de navegação com a **Central de Atendimento — Intranet**.

## Acesso

A aplicação está preparada para publicação como site estático e pode ser utilizada diretamente pelo GitHub Pages.

**Aplicação:**

`https://eubruno-coder.github.io/escala/`

## Status do projeto

**Versão atual: V1 — Interface funcional**

A versão atual concentra-se na experiência de uso da escala e no acompanhamento da jornada em tempo real.

### Recursos disponíveis

- Relógio em tempo real;
- acompanhamento do status da jornada;
- contagem regressiva para eventos;
- indicação de entrada e saída;
- visualização do progresso da jornada;
- linha do tempo de eventos;
- visão semanal da escala;
- edição/configuração da escala;
- identificação básica do operador;
- tema claro e escuro;
- interface responsiva;
- funcionamento sem backend na V1.

## Integração com a Central de Atendimento

O Sistema de Escalas foi estruturado para funcionar como um módulo independente dentro do ecossistema da **Central de Atendimento — Intranet**.

Na intranet, o sistema é disponibilizado em **Links Rápidos**, permitindo que o operador acesse a ferramenta de escala sem abandonar a estrutura principal da Central.

```text
Central de Atendimento — Intranet
                │
                ├── Atendimento
                ├── Scripts
                ├── Links Rápidos
                │       └── Sistema de Escalas
                │
                └── Sistema de Escalas
                        ├── Jornada
                        ├── Pausas
                        ├── Linha do tempo
                        └── Escala semanal
```

A integração atual é principalmente de **navegação e ecossistema**. O Sistema de Escalas continua sendo uma aplicação independente, o que reduz o acoplamento entre os projetos e facilita sua evolução.

## Conceito de produto

A proposta do sistema é transformar uma informação normalmente apresentada de forma estática em uma **interface operacional de acompanhamento da jornada**.

O usuário deve conseguir identificar rapidamente:

- onde está dentro da jornada;
- qual é o próximo evento;
- quanto tempo falta para o próximo evento;
- quais pausas estão previstas;
- como está organizada a semana;
- quais horários estão configurados.

A interface utiliza uma linguagem visual inspirada em **painéis operacionais**, com destaque para estados, contadores e eventos.

## Arquitetura

A V1 utiliza uma arquitetura propositalmente simples: toda a aplicação está concentrada no `index.html`.

```text
escala/
└── index.html
```

O arquivo contém a estrutura HTML, estilos CSS e lógica JavaScript necessários para a execução da versão atual.

Essa abordagem reduz a complexidade inicial e facilita o deploy em hospedagem estática. Conforme o projeto evoluir, a estrutura poderá ser modularizada.

### Arquitetura planejada

```text
escala/
├── index.html
├── README.md
├── docs/
│   ├── ARQUITETURA.md
│   └── REGRAS-E-CONFORMIDADE.md
├── css/
│   └── style.css
├── js/
│   ├── app.js
│   ├── escala.js
│   ├── usuario.js
│   └── armazenamento.js
└── assets/
    └── ...
```

> A estrutura acima representa a evolução planejada e não deve ser interpretada como a estrutura atualmente existente na V1.

## Interface e identidade visual

A interface atual utiliza uma linguagem visual própria, com dois modos de apresentação:

### Tema claro

Pensado para o uso durante o expediente, com fundo claro, painéis de alto contraste e indicadores de estado.

### Tema escuro

Pensado como um modo de operação alternativo, com fundo escuro, elementos de destaque e estética inspirada em consoles operacionais.

A interface utiliza **Inter** para elementos de leitura e **JetBrains Mono** para horários, contadores e informações de caráter operacional.

## Conformidade e parâmetros de jornada

O sistema pode trabalhar com diferentes configurações de horários e pausas. Entretanto, **uma configuração existente na aplicação não representa automaticamente uma regra legal ou uma certificação de conformidade**.

Quando utilizado em atividades sujeitas a requisitos específicos de jornada, pausas ou intervalos, os parâmetros devem ser validados conforme:

- legislação vigente;
- normas regulamentadoras aplicáveis;
- instrumentos coletivos;
- contrato e regras internas da organização;
- características efetivas da atividade exercida.

Para contextos de teleatendimento/telemarketing, a **NR-17, Anexo II**, deve ser considerada como referência normativa aplicável quando o enquadramento legal corresponder à atividade.

> O projeto possui finalidade tecnológica e operacional. A configuração definitiva de jornadas e pausas deve ser validada pelos responsáveis técnicos, operacionais e jurídicos competentes.

## Segurança e privacidade

A V1 não depende de banco de dados ou autenticação centralizada.

Caso o projeto passe a armazenar dados pessoais, deverão ser incorporados mecanismos adequados de segurança, controle de acesso, retenção e exclusão, considerando a legislação brasileira aplicável, incluindo a **LGPD**.

Não devem ser publicados no repositório:

- senhas;
- tokens;
- chaves de API;
- credenciais;
- dados pessoais desnecessários;
- informações internas que não tenham autorização para publicação.

## Roadmap

### V1 — Interface funcional

- [x] Visualização da jornada
- [x] Relógio em tempo real
- [x] Contagem regressiva
- [x] Status da jornada
- [x] Linha do tempo
- [x] Escala semanal
- [x] Editor/configuração de escala
- [x] Identificação básica do operador
- [x] Tema claro/escuro
- [x] Layout responsivo
- [x] Publicação como aplicação web estática
- [x] Integração de navegação com a Central de Atendimento

### V2 — Persistência e usuários

- [ ] Separação de HTML, CSS e JavaScript
- [ ] Banco de dados
- [ ] Cadastro de usuários
- [ ] Identificação persistente
- [ ] Salvamento das escalas
- [ ] Recuperação das configurações
- [ ] Controle de permissões
- [ ] Histórico de alterações

### V3 — Gestão

- [ ] Painel administrativo
- [ ] Gestão de equipes
- [ ] Gestão de múltiplas escalas
- [ ] Auditoria de alterações
- [ ] Relatórios
- [ ] Configuração centralizada de parâmetros
- [ ] Integração mais profunda com a Intranet

### V4 — Plataforma

- [ ] API
- [ ] Banco de dados estruturado
- [ ] Autenticação segura
- [ ] Controle de acesso por perfil
- [ ] Logs e auditoria
- [ ] Backup e recuperação
- [ ] Arquitetura preparada para múltiplas unidades/equipes

## Filosofia técnica

O desenvolvimento segue alguns princípios:

- **simplicidade:** reduzir dependências e complexidade desnecessária;
- **baixo custo:** priorizar infraestrutura gratuita ou de baixo custo quando viável;
- **modularidade:** permitir evolução gradual sem reescrever o produto inteiro;
- **usabilidade:** priorizar leitura rápida das informações operacionais;
- **transparência:** diferenciar parâmetros configuráveis de requisitos externos;
- **segurança:** preparar a arquitetura para autenticação, autorização e auditoria;
- **manutenibilidade:** manter o código preparado para futuras evoluções.

## Desenvolvimento colaborativo

Este projeto foi desenvolvido com apoio de **inteligência artificial** em atividades de concepção, arquitetura, revisão, documentação e implementação.

A autoria do repositório, das decisões de produto e da direção do projeto permanece com o responsável pelo repositório.

A utilização de assistência de IA não constitui, por si só, sociedade, vínculo empregatício, representação jurídica ou parceria comercial.

## Licenciamento

A licença definitiva do projeto ainda será definida pelo responsável pelo repositório.

Enquanto não houver uma licença explícita no repositório, o código **não deve ser presumido como estando sob uma licença open source específica**.

## Changelog

### V1 — 2026

- Estrutura inicial da aplicação web;
- criação do acompanhamento de jornada;
- implementação de contadores e status;
- criação da linha do tempo;
- implementação da escala semanal;
- editor/configuração da escala;
- identificação básica do operador;
- implementação de tema claro e escuro;
- preparação para publicação em GitHub Pages;
- integração de navegação com a Central de Atendimento.

## Próximas prioridades

A evolução recomendada do projeto é:

1. modularizar o `index.html`;
2. criar documentação técnica separada;
3. definir o modelo de dados da escala;
4. adicionar persistência local antes de introduzir um backend;
5. avaliar autenticação e banco de dados;
6. aprofundar a integração com a Central de Atendimento;
7. estabelecer governança e política de licenciamento antes de ampliar a distribuição.

## Referências oficiais

- Ministério do Trabalho e Emprego — NR-17;
- NR-17 — Anexo II — Teleatendimento/Telemarketing.

As referências normativas devem ser consultadas sempre em suas versões oficiais e vigentes antes da configuração de regras no sistema.

---

**Projeto:** Sistema de Escalas  
**Repositório:** `eubruno-coder/escala`  
**Versão atual:** V1  
**Status:** Em desenvolvimento contínuo  
**Ecossistema:** Central de Atendimento — Intranet
