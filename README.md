# DeskHelpFront

## 📋 Tecnologias

- **Angular 20**
- **Node.js 22**
- **Angular Material** (UI Components)
- **RxJS** (Programação reativa)
- **NgRx** (Opcional - State Management)
- **ESLint** + **Prettier** (Padronização)

## ⚙️ Configuração do Ambiente

### Pré-requisitos
- Node.js 22.x
- npm 10+ ou yarn 1.22+
- Angular CLI 20+

### Instalação
1. Clone o repositório:
   ```bash
   git clone https://github.com/EmersonBranch/desk-help-front.git
   ```
2. Instale dependências:
   ```bash
   npm install
   # ou
   yarn install
   ```

3. Configure a API:
   - Altere `environment.ts` com a URL do backend

4. Execute a aplicação:
   ```bash
   ng serve
   ```
   Acesse: `http://localhost:4200`

## 🏗️ Estrutura do Projeto
```
src/
├── app/
│   ├── core/           # Serviços globais
│   ├── modules/        # Feature modules
│   ├── shared/         # Componentes compartilhados
│   ├── assets/         # Imagens/fontes
│   ├── styles/         # CSS global
│   └── app.component.ts
├── environments/       # Configurações por ambiente
└── ...
```

## 🛠️ Comandos Úteis
```bash
# Rodar em modo desenvolvimento
ng serve

# Build para produção
ng build --configuration=production

# Rodar testes unitários
ng test

# Lint do projeto
ng lint
```

## 🌐 Configuração de Proxy
Para evitar CORS durante o desenvolvimento, configure `proxy.conf.json`:
```json
{
  "/api": {
    "target": "http://localhost:8080",
    "secure": false
  }
}
```

## 🤝 Contribuição
Siga o fluxo Git:
1. Branchs devem ser criadas a partir de `prod`
2. Push inicial para `dev`
3. PRs devem ser abertos para `stage`
```
