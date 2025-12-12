<div align="center">
  <img src="./assets/eject_labs_logo.svg" alt="Logo EJECT LABS" width="440" />
</div>

<div align="center">
    <p><b>Laboratório Contínuo de Inovação da EJECT</b></p>
    Ideias reais. Produtos reais. Impacto real.
</div>

<div align="center">
  <img src="https://img.shields.io/badge/STATUS-ATIVO-00C853?style=for-the-badge" />
  <img src="https://img.shields.io/badge/PROJETOS-EM%20ANDAMENTO-2979FF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/TRILHA-INTEGRADA-7C4DFF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/FOCO-INOVA%C3%87%C3%83O-FF9100?style=for-the-badge" />
  <img src="https://img.shields.io/badge/DOCUMENTA%C3%87%C3%83O-OBRIGAT%C3%93RIA-00E5FF?style=for-the-badge" />
</div>

---

## ✨ Visão, Propósito & Objetivos do EJECT LABS

O **EJECT LABS** é o laboratório de inovação contínua da EJECT, criado para transformar **ideias em soluções reais** de forma estruturada, prática e com impacto direto no negócio.

Seus principais objetivos são:

* ✅ Promover a inovação contínua de forma organizada
* ✅ Criar produtos de prateleira com potencial real de mercado
* ✅ Desenvolver sistemas internos que otimizem processos da EJECT
* ✅ Gerar desafios práticos e reais para a trilha de nivelamento
* ✅ Construir um portfólio técnico sólido para os membros

No EJECT LABS, toda ideia tem como norte se tornar **produto, sistema, melhoria de processo ou desafio técnico com valor real**.

---

## 🔬 Como o LABS Funciona

O LABS é uma iniciativa criada para promover desenvolvimento ágil, modular e colaborativo dentro da EJECT. A ideia é reduzir esforços repetitivos e permitir que nossos membros foquem no que realmente importa: inovação, criatividade e construção de novas ideias.

Este repositório é organizado em módulos de backend e frontend. Assim, para cada novo projeto, é possível:

- Utilizar uma base padrão de frontend, inspirada no mockup do CVB;

- Reaproveitar módulos já desenvolvidos de backend, acelerando o processo;

- Concentrar o desenvolvimento apenas nas lógicas específicas de cada ideia.


Dessa forma, o LABS cria um ambiente mais eficiente e escalável, permitindo que novos projetos nasçam mais rápido e com mais qualidade.

---

## 🗂️ Organização do Repositório

```bash
EJECT-LABS/
│
├── backend/
│   ├── modules/
│   │   ├── auth/
│   │   ├── email/
│   │   ├── utils/
│   │   └── crud/
│   └── base_project/
│       └── django_base_template/
│
├── frontend/
│   ├── ui/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── styles/
│   │   └── theme.js
│   └── base/
│       └── react_base_template/
│
└── docs/
```

---

## 🤝 Como usar o EJECT LABS e como colaborar?

🚀 Como Utilizar o EJECT LABS

Este guia apresenta o passo a passo para iniciar rapidamente um novo projeto utilizando o EJECT LABS, garantindo padronização visual e reutilização dos módulos backend e frontend.


---

🟦 1. Clonando o EJECT LABS

git clone https://github.com/ejectlabs/ejectlabs-monorepo.git
echo "cd ejectlabs-monorepo"


---

🟩 2. Instalando os Módulos Backend (Django)

Cada módulo está localizado em backend/modules/ e pode ser instalado diretamente via pip.

Exemplo — instalando o módulo de autenticação:

pip install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=backend/modules/auth"

Instale quantos módulos desejar:

pip install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=backend/modules/utils"
pip install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=backend/modules/email"

Depois, adicione no settings.py do seu projeto Django:

INSTALLED_APPS = [
    "auth_module",
    "email_module",
    "utils_module",
]


---

🟦 3. Criando um Novo Projeto Backend Base

O monorepo possui um template Django em:

backend/base/base_django

Para iniciar um backend usando a base EJECT:

cp -r backend/base/base_django my_new_api
cd my_new_api
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver


---

🟩 4. Instalando o Frontend Base (React)

Dentro do monorepo há um template pronto em:

frontend/base/react_base

Para iniciar um novo frontend:

cp -r frontend/base/react_base my_new_frontend
cd my_new_frontend
npm install
npm run dev


---

🧱 5. Utilizando os Componentes da UI

Todos os componentes reutilizáveis estão em:

frontend/ui

Para instalá-los em qualquer projeto:

npm install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=frontend/ui"

Exemplo de uso:

import { Button } from "@ejectlabs/ui";

export default function Home() {
  return <Button>Entrar</Button>;
}


---

🧪 6. Estrutura Recomendada de Desenvolvimento

Use o frontend/base para iniciar o layout.

Use os módulos backend para funcionalidades prontas.

Use o UI system para manter o padrão EJECT.

Mantenha tudo versionado no monorepo.



---

🎯 7. Objetivo

O EJECT LABS serve para:

acelerar o desenvolvimento,

padronizar design e arquitetura,

evitar retrabalho,

criar produtos com identidade visual unificada,

dar maturidade técnica aos projetos da EJECT.


🤝 Guia de Contribuição — EJECT LABS

Obrigado por contribuir com o EJECT LABS! Este guia explica como colaborar de forma padronizada e eficiente no monorepo. Nosso objetivo é garantir qualidade, consistência e evolução contínua dos módulos backend, frontend e da base de projetos.

---

## 🎓 Integração com a Trilha de Nivelamento

Os projetos do EJECT LABS são usados como:

* ✅ Desafios finais por nível
* ✅ Projetos práticos
* ✅ Casos reais de desenvolvimento

Todo esforço aplicado gera **valor direto para a EJECT**.

---

## 🚦 Projetos em Andamento no EJECT LABS

Aqui você encontra a vitrine oficial dos projetos que estão sendo idealizados, desenvolvidos, testados e consolidados dentro do **EJECT LABS**.

Todos os projetos listados abaixo possuem acesso direto ao seu **README**, **repositório**, **documentação**, **backlog** e **status de execução**, garantindo total transparência, rastreabilidade e padronização do processo de inovação.

### 🧠 Em Ideação / Planejamento ![Status](https://img.shields.io/badge/status-ativo-success)

| Projeto | README | Repositório | Status |
|--------|--------|-------------|--------|
| 🧩 SAM — Sistema de Advertência de Membros | [Acessar Escopo](LINK) | [Acessar Repositorio](LINK) | Em andamento |


### ✅ Em Desenvolvimento ![Status](https://img.shields.io/badge/status-aguardando-yellow)

🚧 Nenhum projeto no momento

| Projeto | README | Repositório | Status |
|--------|--------|-------------|--------|
| — | — | — | — |

### 🟡 Em Validação ![Status](https://img.shields.io/badge/status-aguardando-yellow)

🚧 Nenhum projeto no momento

| Projeto | README | Repositório | Status |
|--------|--------|-------------|--------|
| — | — | — | — |


### 🏁 Concluídos ![Status](https://img.shields.io/badge/status-aguardando-yellow)

🚧 Nenhum projeto no momento

| Projeto | README | Repositório | Status |
|--------|--------|-------------|--------|
| — | — | — | — | 

---

## 👥 Quem Participa

* Trainees
* Membros da trilha
* Coordenadores
* Lideranças técnicas

Todos podem propor ideias, desenvolver projetos e documentar soluções.

---

## 🤝 Como Contribuir

1. Escolha um projeto ativo
2. Laboratório Contínuo de Inovação da EJECTLeia a documentação
3. Crie uma branch
4. Desenvolva
5. Documente
6. Abra um Pull Request

<div align="center">
    <p><b>🧠 EJECT LABS — Onde ideias deixam de ser conceito e viram soluções reais.</b></p>

</div>
