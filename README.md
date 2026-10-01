# Bee Well — Plataforma de Acompanhamento Emocional

O **Bee Well** é uma plataforma web desenvolvida para apoiar o acompanhamento emocional por meio do registro, organização e visualização de informações relacionadas ao bem-estar do usuário.

A solução foi projetada com foco em **privacidade, segurança da informação, experiência do usuário e organização dos dados**, oferecendo ambientes distintos para pacientes e profissionais.

> Projeto autoral em desenvolvimento. O código-fonte principal permanece privado e este repositório é destinado à apresentação técnica e documentação do projeto.

---

## Sobre o projeto

O acompanhamento emocional envolve informações pessoais que precisam ser organizadas de maneira segura, acessível e compreensível.

O Bee Well foi idealizado para centralizar esse processo em uma plataforma digital, permitindo que usuários acompanhem seus registros ao longo do tempo e que profissionais tenham acesso às informações disponibilizadas conforme as permissões definidas no sistema.

A arquitetura do projeto foi planejada considerando desde o início aspectos como:

- separação de perfis;
- controle de acesso;
- proteção de informações sensíveis;
- organização do histórico;
- escalabilidade;
- experiência do usuário.

---

## Perfis de acesso

### Paciente

O paciente utiliza a plataforma para registrar e acompanhar informações relacionadas ao seu bem-estar emocional.

Entre as funcionalidades previstas estão:

- registro de humor;
- acompanhamento de ansiedade;
- acompanhamento do sono;
- consulta ao próprio histórico;
- gerenciamento das informações pessoais.

### Profissional

O perfil profissional possui uma visão voltada ao acompanhamento dos usuários vinculados, respeitando as regras de acesso e privacidade estabelecidas pela aplicação.

O objetivo é oferecer uma interface organizada para consulta e acompanhamento das informações disponibilizadas pelo paciente.

---

## Fluxo principal

```text
Paciente
   ↓
Registra informações de acompanhamento
   ↓
Dados são processados pela aplicação
   ↓
Informações sensíveis são protegidas
   ↓
Dados são armazenados no PostgreSQL
   ↓
Histórico é disponibilizado conforme
perfil e permissões de acesso
```

---

## Principais funcionalidades

- Cadastro e autenticação de usuários
- Diferentes perfis de acesso
- Registro de informações emocionais
- Histórico de acompanhamento
- Organização dos registros do usuário
- Controle de acesso baseado em perfil
- Persistência de dados em banco relacional
- Proteção de informações sensíveis
- Interface responsiva
- Estrutura preparada para novas funcionalidades

---

## Segurança e privacidade

Segurança é um dos pilares do Bee Well devido à natureza das informações processadas pela plataforma.

O projeto contempla mecanismos como:

- criptografia **AES-256-GCM** para proteção de informações sensíveis;
- controle de acesso baseado no perfil do usuário;
- separação entre interface, regras de negócio e persistência;
- tratamento adequado dos dados antes do armazenamento;
- arquitetura preparada para evolução dos mecanismos de autenticação e autorização.

O objetivo é reduzir a exposição desnecessária das informações e aplicar boas práticas de desenvolvimento seguro desde a estruturação do sistema.

---

## Tecnologias

### Frontend

- Next.js
- React
- TypeScript

### Backend

- Node.js
- Prisma ORM

### Banco de dados

- PostgreSQL

### Segurança

- AES-256-GCM

### Versionamento

- Git
- GitHub

---

## Arquitetura

O Bee Well utiliza uma arquitetura dividida em camadas para manter responsabilidades bem definidas e facilitar a manutenção e evolução do sistema.

```text
┌──────────────────────────┐
│        Usuário           │
│  Paciente / Profissional │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│        Frontend          │
│   Next.js + TypeScript   │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│      Backend / API       │
│         Node.js          │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│        Prisma ORM        │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│       PostgreSQL         │
└──────────────────────────┘
```

---

## Diferenciais do projeto

### Segurança desde a arquitetura

A proteção dos dados não foi tratada apenas como uma etapa posterior do desenvolvimento. O projeto considera segurança e privacidade desde a estruturação da aplicação.

### Separação de perfis

Paciente e profissional possuem responsabilidades e níveis de acesso diferentes dentro do sistema.

### Organização do histórico

Os registros são estruturados para permitir acompanhamento ao longo do tempo de forma clara e organizada.

### Arquitetura escalável

A separação entre frontend, backend e banco de dados permite a evolução independente das diferentes partes da aplicação.

### Foco em experiência do usuário

A interface foi pensada para tornar o registro e a consulta das informações simples, reduzindo complexidade para o usuário final.

---

## Status do projeto

**Em desenvolvimento**

### Implementado

- [x] Estrutura inicial do projeto
- [x] Frontend
- [x] Principais interfaces
- [x] Definição dos perfis de usuário
- [x] Estruturação inicial do banco de dados
- [x] Estratégia para proteção de dados sensíveis

### Em desenvolvimento

- [ ] Finalização do backend
- [ ] Integração completa com PostgreSQL
- [ ] Regras de negócio
- [ ] Autenticação e autorização
- [ ] Testes automatizados

---

## Roadmap

### Fase 1 — Estrutura da aplicação

- Desenvolvimento das interfaces
- Definição dos perfis
- Modelagem inicial dos dados

### Fase 2 — Backend e integração

- APIs
- Prisma ORM
- PostgreSQL
- Integração frontend/backend

### Fase 3 — Segurança

- Proteção de informações sensíveis
- Controle de acesso
- Evolução da autenticação

### Fase 4 — Qualidade

- Testes automatizados
- Tratamento de erros
- Validação das regras de negócio
- Melhorias de desempenho

### Fase 5 — Evolução

- Dashboard de acompanhamento
- Novas formas de visualização do histórico
- Melhorias de UX
- Deploy da aplicação

---

## Objetivo técnico

O Bee Well também funciona como um projeto prático para aplicação e aprofundamento de conhecimentos em:

- Desenvolvimento Full Stack
- Next.js
- React
- TypeScript
- Node.js
- APIs
- PostgreSQL
- Prisma ORM
- Modelagem de dados
- Segurança da Informação
- Arquitetura de Software
- Experiência do Usuário

---

## Autora

**Leticia Pastorini**

Desenvolvimento, arquitetura, modelagem e evolução do projeto.
