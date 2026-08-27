# Sistema de Escalas

> Plataforma em desenvolvimento para organização, visualização e gerenciamento de jornadas, escalas e pausas de trabalho.

[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-orange)](#status-do-projeto)
[![Versão](https://img.shields.io/badge/versão-V1-blue)](#roadmap)
[![Licença](https://img.shields.io/badge/licença-a%20definir-lightgrey)](#licenciamento)

## Sobre o projeto

O **Sistema de Escalas** nasceu com uma proposta simples: transformar a gestão de escalas e pausas em uma experiência visual, acessível e fácil de manter.

A primeira versão funciona como uma aplicação web independente, concentrada em um único `index.html`, com interface responsiva, acompanhamento da jornada em tempo real, contador de eventos, linha do tempo, visão semanal, edição da escala e alternância entre tema claro e escuro.

O projeto está sendo construído de forma incremental, priorizando baixo custo de operação, facilidade de manutenção e possibilidade de evolução para uma arquitetura com persistência de dados e identificação de usuários.

## Conceito

A plataforma foi pensada para funcionar como uma **camada de organização da jornada**, permitindo que o usuário visualize de forma objetiva:

- horário de entrada e saída;
- duração da jornada configurada;
- status atual da jornada;
- próximo evento ou pausa;
- contagem regressiva em tempo real;
- progresso da jornada;
- linha do tempo;
- escala semanal;
- configuração dos horários;
- identificação básica do operador;
- tema claro ou escuro.

O objetivo não é apenas mostrar horários, mas criar uma base que possa evoluir para uma solução de gestão de escalas mais completa.

## Desenvolvimento colaborativo

Este repositório representa um **projeto desenvolvido de forma colaborativa entre o autor do repositório e a assistência de inteligência artificial utilizada durante o processo de concepção, arquitetura, documentação, revisão e evolução da plataforma**.

A autoria do repositório e das decisões de produto permanece com seu responsável. A participação da IA constitui assistência técnica e de desenvolvimento, não configurando, por si só, sociedade, vínculo empregatício, representação jurídica ou parceria comercial.

## Estado atual

A versão atual é identificada como **V1** e possui uma implementação front-end independente.

A estrutura atualmente publicada contém o arquivo principal `index.html`. fileciteturn1file0

Entre os recursos já presentes estão o relógio, acompanhamento de status, contador regressivo, informações de entrada/saída, linha do tempo, escala semanal, editor de escala, identificação do operador e modo escuro. fileciteturn2file0 fileciteturn3file0

## Conformidade e regras de utilização

A plataforma é desenvolvida considerando requisitos e referências regulatórias aplicáveis ao contexto em que for utilizada, especialmente quando destinada a atividades de teleatendimento/telemarketing.

A **NR-17**, em seu Anexo II, estabelece requisitos específicos para trabalho em teleatendimento/telemarketing, incluindo organização do trabalho, pausas e intervalos. O texto oficial atualmente disponibilizado pelo Ministério do Trabalho e Emprego deve ser utilizado como referência normativa. [NR-17 — Ministério do Trabalho e Emprego](https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/participacao-social/conselhos-e-orgaos-colegiados/comissao-tripartite-paritaria-permanente/normas-regulamentadora/normas-regulamentadoras-vigentes/norma-regulamentadora-no-17-nr-17) citeturn0search0turn0search15

**Importante:** a existência da plataforma não significa, por si só, certificação de conformidade trabalhista ou ergonômica. A configuração de jornadas, pausas, intervalos e demais parâmetros deve ser validada de acordo com a legislação vigente, atividade exercida, contrato, instrumentos coletivos aplicáveis e políticas da organização.

### Princípios de conformidade

1. Os parâmetros de jornada não devem ser configurados de maneira deliberadamente incompatível com as normas aplicáveis.
2. As pausas e intervalos devem respeitar os requisitos legais e regulamentares pertinentes ao contexto de utilização.
3. Alterações administrativas devem ser realizadas somente por pessoas autorizadas.
4. A plataforma não deve ser utilizada para suprimir direitos, impedir pausas obrigatórias ou induzir o trabalhador a descumprir regras de saúde e segurança.
5. Registros e configurações devem ser preservados de forma responsável quando a aplicação passar a utilizar armazenamento persistente.
6. Qualquer atualização normativa relevante deve ser analisada antes de ser incorporada como regra automática do sistema.

### Uso indevido e descumprimento

O uso da plataforma em desacordo com sua finalidade, com as regras internas de uma organização ou com a legislação aplicável é de responsabilidade de quem realizar, autorizar ou manter a configuração indevida.

Dependendo do contexto, alterações ou utilização indevida poderão resultar nas **medidas administrativas, contratuais ou legais cabíveis**, observados o devido processo, a legislação aplicável e as competências de cada responsável.

Este projeto não cria novas penalidades nem substitui as sanções previstas em lei, contrato, regulamento interno ou instrumento coletivo.

## Atenção sobre os parâmetros de pausas

O sistema possui liberdade técnica para trabalhar com diferentes configurações de jornada. Entretanto, **uma configuração existente no software não deve ser interpretada automaticamente como uma regra legal**.

Para atividades enquadradas no Anexo II da NR-17, o texto oficial prevê, entre outros requisitos, duas pausas de 10 minutos e intervalo de 20 minutos para repouso e alimentação, além de outras disposições específicas. citeturn0search13turn0search15

Por isso, jornadas específicas, como 6h20, 8h12 ou outras modalidades eventualmente adotadas pelo projeto, devem ser tratadas como **parâmetros de configuração** e validadas juridicamente/operacionalmente antes de serem apresentadas como conformes a uma norma.

## Arquitetura planejada

A V1 utiliza uma estrutura simples para reduzir barreiras de implantação. A evolução prevista é separar gradualmente as responsabilidades:

```text
escala/
├── index.html
├── README.md
├── docs/
│   ├── REGRAS-E-CONFORMIDADE.md
│   └── ARQUITETURA.md
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

A separação acima representa a **arquitetura planejada**, não a estrutura obrigatoriamente existente na V1.

## Próxima evolução

### V1 — Interface funcional

- [x] Visualização da jornada
- [x] Relógio em tempo real
- [x] Contagem regressiva
- [x] Status da jornada
- [x] Linha do tempo
- [x] Escala semanal
- [x] Editor de escala
- [x] Identificação básica do operador
- [x] Tema claro/escuro
- [x] Layout responsivo

### V2 — Persistência e usuários

- [ ] Banco de dados
- [ ] Cadastro de usuários
- [ ] Identificação persistente
- [ ] Salvamento das escalas
- [ ] Recuperação da configuração do usuário
- [ ] Controle de permissões
- [ ] Histórico de alterações

### V3 — Gestão

- [ ] Painel administrativo
- [ ] Gestão de equipes
- [ ] Gestão de múltiplas escalas
- [ ] Auditoria de alterações
- [ ] Relatórios
- [ ] Configuração centralizada de parâmetros

### V4 — Escalabilidade

- [ ] Separação completa entre front-end e back-end
- [ ] API
- [ ] Banco de dados estruturado
- [ ] Autenticação segura
- [ ] Controle de acesso por perfil
- [ ] Logs e auditoria
- [ ] Rotinas de backup

## Filosofia técnica

O projeto prioriza:

- **baixo custo:** utilizar recursos gratuitos ou de baixo custo sempre que tecnicamente viável;
- **simplicidade:** evitar dependências desnecessárias;
- **acessibilidade:** permitir que a plataforma seja compreendida e utilizada sem treinamento complexo;
- **manutenção:** facilitar alterações futuras nas regras e horários;
- **transparência:** deixar claro quais parâmetros são configuráveis e quais são requisitos externos;
- **segurança:** evoluir gradualmente para autenticação, autorização, persistência e auditoria;
- **conformidade:** não transformar uma configuração de software em falsa garantia de conformidade legal.

## Segurança e dados

Quando o sistema passar a armazenar informações pessoais, deverão ser definidos controles apropriados para coleta, finalidade, acesso, alteração, retenção e exclusão dos dados.

A evolução para banco de dados deverá considerar, conforme aplicável, princípios de segurança da informação e a legislação brasileira de proteção de dados, incluindo a LGPD.

Nenhuma senha, chave de API, token, credencial ou dado sensível deve ser armazenado diretamente no código-fonte ou publicado no repositório.

## Licenciamento

A licença definitiva do projeto ainda será definida pelo responsável pelo repositório.

Enquanto não houver uma licença explícita neste repositório, o código não deve ser presumido como estando sob uma licença open source específica.

## Responsabilidade

Este repositório é um projeto de software em desenvolvimento. A documentação técnica e as referências regulatórias têm finalidade informativa e de orientação de projeto.

A implementação em ambiente real deve ser submetida às validações técnicas, operacionais e jurídicas necessárias, especialmente quando envolver jornada de trabalho, pausas, dados pessoais ou obrigações regulatórias.

## Referências oficiais

- [Ministério do Trabalho e Emprego — NR-17](https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/participacao-social/conselhos-e-orgaos-colegiados/comissao-tripartite-paritaria-permanente/normas-regulamentadora/normas-regulamentadoras-vigentes/norma-regulamentadora-no-17-nr-17)
- [NR-17 — Anexo II — Teleatendimento/Telemarketing](https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/participacao-social/conselhos-e-orgaos-colegiados/comissao-tripartite-paritaria-permanente/arquivos/normas-regulamentadoras/nr-17-anexo-ii-teleatendimento-atualizado-2021.pdf)

---

**Projeto:** Sistema de Escalas  
**Repositório:** `eubruno-coder/escala`  
**Versão atual:** V1  
**Status:** Em desenvolvimento contínuo
