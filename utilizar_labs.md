# 🚀 Como Utilizar o EJECT LABS

> Este guia apresenta o passo a passo para iniciar rapidamente um novo projeto utilizando o EJECT LABS, garantindo padronização visual e reutilização dos módulos backend e frontend.

---

## 🟦 1. Clonando o EJECT LABS

```bash
git clone https://github.com/ejectlabs/ejectlabs-monorepo.git
echo "cd ejectlabs-monorepo"
```

---

## 🟩 2. Instalando os Módulos Backend (Django)

Cada módulo está localizado em backend/modules/ e pode ser instalado diretamente via pip.

Exemplo — instalando o módulo de autenticação:

```bash
pip install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=backend/modules/auth"
```

Instale quantos módulos desejar:

```bash
pip install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=backend/modules/utils"
pip install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=backend/modules/email"
```

Depois, adicione no settings.py do seu projeto Django:

```py
INSTALLED_APPS = [
    "auth_module",
    "email_module",
    "utils_module",
]

```

---

## 🟦 3. Criando um Novo Projeto Backend Base

O monorepo possui um template Django em:

> backend/base/base_django


Para iniciar um backend usando a base EJECT:

```bash
cp -r backend/base/base_django my_new_api
cd my_new_api
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

---

## 🟩 4. Instalando o Frontend Base (React)

Dentro do monorepo há um template pronto em:

> frontend/base/react_base

Para iniciar um novo frontend:

```bash
cp -r frontend/base/react_base my_new_frontend
cd my_new_frontend
npm install
npm run dev
```

---

## 🧱 5. Utilizando os Componentes da UI

Todos os componentes reutilizáveis estão em:

> frontend/ui

Para instalá-los em qualquer projeto:

```bash
npm install "git+https://github.com/ejectlabs/ejectlabs-monorepo.git#subdirectory=frontend/ui"
```

Exemplo de uso:

```bash
import { Button } from "@ejectlabs/ui";

export default function Home() {
  return <Button>Entrar</Button>;
}
```


---

## 🧪 6. Estrutura Recomendada de Desenvolvimento

- Use o frontend/base para iniciar o layout.

- Use os módulos backend para funcionalidades prontas.

- Use o UI system para manter o padrão EJECT.

Mantenha tudo versionado no EJECT LABS.
