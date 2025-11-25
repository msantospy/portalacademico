Portal Acadêmico

Descrição curta: repositório com frontend (Vite) e um diretório `backend/` com o código do servidor. O frontend está configurado no nível raiz com Vite; o backend existe em `backend/` (possui a estrutura de pastas, mas não tem scripts ou dependências definidos no `backend/package.json`).

---

## Estrutura do projeto

Raiz:

```
index.html
package.json          # frontend (Vite) - scripts: dev, build, preview
public/
src/                  # frontend source (main.js, counter.js, style.css)
backend/              # backend: src/ (app.js, server.js, models/, routes/, services/)
README.md
```

Observação: o `backend/package.json` no repositório atual está vazio — antes de iniciar o backend confirme se há scripts e dependências definidas (ou siga as instruções de setup abaixo).

---

## Requisitos

- Node.js (recomendo >= 16/18)
- npm ou yarn / pnpm
- Git
- Docker (opcional)

---

## Como inicializar (texto para colar no Notion)

### Frontend (onde está o Vite)

1. Abra um terminal na raiz do projeto (onde está o `package.json` com Vite).
2. Instale dependências:

```powershell
npm install
# ou
yarn
# ou
pnpm install
```


Porta padrão do Vite: 5173 (ver saída do comando `npm run dev`).

---

### Backend (pasta `backend/`)

Observação: no estado atual do repositório, `backend/package.json` está vazio

---

### Rodar tudo junto

Abra dois terminais (um para frontend e outro para backend) e execute os comandos de dev em cada um. Alternativamente, adicione uma solução como `concurrently` ou `docker-compose` para rodar ambos com um único comando.

Exemplo simples (PowerShell) - Terminal 1 (frontend):

```powershell
cd C:\caminho\para\projeto
npm run dev
```

Terminal 2 (backend):

```powershell
cd C:\caminho\para\projeto\backend
npm run dev
```

---

### Observações finais

- Adapte nomes de scripts, dependências e portas conforme o `package.json` de cada pasta.