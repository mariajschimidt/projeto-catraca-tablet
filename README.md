
---

# 🎫 Catraca Touch | Movement Academy

### *Sistema de Check-in por CPF — Interface Touch-Screen para Validação de Acesso em Academias*

Bem-vindo ao **Catraca Touch**, um terminal digital interativo desenvolvido para academias que desejam agilizar e modernizar o processo de entrada de alunos. Com um design otimizado para tablets e quiosques touch-screen, o sistema permite a digitação do CPF em um teclado virtual intuitivo e realiza a validação em tempo real com a API de backend, informando imediatamente se o acesso está **liberado** ou **bloqueado**.

---

## ✨ Demonstração Online

| Projeto | Link |
|---------|------|
| 🎫 **Catraca Touch (Frontend)** | [projeto-catraca-tablet.vercel.app](https://projeto-catraca-tablet.vercel.app/) |
| ⚙️ **Backend API** | [catraca-api.vercel.app](https://catraca-api.vercel.app) |

> *O sistema consome a mesma API do painel administrativo, garantindo sincronização total dos dados.*

---

## 🛠️ Tecnologias Utilizadas

### Frontend
<div align="left">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="TailwindCSS" />
  <img src="https://img.shields.io/badge/Font_Awesome-528DD7?style=for-the-badge&logo=fontawesome&logoColor=white" alt="Font Awesome" />
  <img src="https://img.shields.io/badge/Google_Fonts-4285F4?style=for-the-badge&logo=google-fonts&logoColor=white" alt="Google Fonts" />
</div>

### Backend & Infraestrutura
<div align="left">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express.js" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
</div>

### Design & UX para Touch
<div align="left">
  <img src="https://img.shields.io/badge/Touch_Optimized-FF6B6B?style=for-the-badge&logo=hand-touch&logoColor=white" alt="Touch Optimized" />
  <img src="https://img.shields.io/badge/Glassmorphism-8b5cf6?style=for-the-badge&logo=css3&logoColor=white" alt="Glassmorphism" />
  <img src="https://img.shields.io/badge/Responsive-00C4B3?style=for-the-badge&logo=responsive-design&logoColor=white" alt="Responsive" />
  <img src="https://img.shields.io/badge/Kiosk_Mode-000000?style=for-the-badge&logo=screen&logoColor=white" alt="Kiosk Mode" />
</div>

---

## 📸 Visão Geral do Sistema

| Funcionalidade | Descrição |
|----------------|-------------|
| **Teclado Virtual Touch** | Botões grandes e espaçados para digitação fácil em tablets |
| **Máscara de CPF Automática** | Formatação em tempo real: `000.000.000-00` |
| **Validação em Tempo Real** | Consulta à API para verificar status do aluno |
| **Feedback Visual Imediato** | Cores e mensagens claras para acesso liberado/bloqueado |
| **Proteção contra Erros** | Validação de CPF com 11 dígitos antes da consulta |
| **Design Glassmorphism** | Interface moderna com efeito de vidro fosco |
| **Otimizado para Quiosques** | Interface sem rolagem, botões grandes e responsivos |

---

## 🧠 Arquitetura do Projeto

```
┌─────────────────────────────────────────────────────────────┐
│              Catraca Touch (Este Projeto)                    │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐  │
│  │   HTML5     │  │ TailwindCSS │  │  JavaScript (ES6+)  │  │
│  │  Estrutura  │  │  Estilização │  │   Lógica & Fetch    │  │
│  └─────────────┘  └─────────────┘  └─────────────────────┘  │
│                                                               │
│         🖥️ Otimizado para Tablets e Quiosques Touch          │
└─────────────────────────────────────────────────────────────┘
                              │
                              │ HTTP Requests (Fetch API)
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              Backend API (Desenvolvido por @fonseca-felix)   │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐  │
│  │  Node.js    │  │  Express    │  │   JWT Auth          │  │
│  │   Server    │  │   Router    │  │   (Admin Only)      │  │
│  └─────────────┘  └─────────────┘  └─────────────────────┘  │
│                                                               │
│  ┌─────────────────────────────────────────────────────┐    │
│  │              MongoDB / Database                      │    │
│  │         (Persistência de Alunos + Status)           │    │
│  └─────────────────────────────────────────────────────┘    │
│                                                               │
│           🌐 Deploy: catraca-api.vercel.app                  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              Painel Administrativo (Projeto Irmão)           │
│  ┌─────────────────────────────────────────────────────┐    │
│  │  Gestão de Alunos - Cadastro, Edição, Bloqueio      │    │
│  │  🌐 Deploy: projeto-catraca-adm.vercel.app          │    │
│  └─────────────────────────────────────────────────────┘    │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎯 Fluxo de Uso

```
┌────────────────┐
│  Aluno chega   │
│  na academia   │
└───────┬────────┘
        ▼
┌────────────────┐
│ Digita CPF no  │
│ teclado virtual│
└───────┬────────┘
        ▼
┌────────────────┐
│ Pressiona      │
│ "Validar Acesso"│
└───────┬────────┘
        ▼
┌────────────────────────────────────┐
│         API /alunos/:cpf           │
│  Verifica existência e status      │
└───────┬────────────────────────────┘
        ▼
   ┌────┴────┐
   ▼         ▼
┌───────┐ ┌───────┐
│LIBERADO│ │BLOQUEADO│
│ 🟢    │ │ 🔴    │
│Acesso  │ │Acesso  │
│Permitido│ │Negado  │
└───────┘ └───────┘
```

---

## ⚙️ Funcionalidades Técnicas

### 🖱️ Interface Touch-Otimizada
- **Botões grandes** (mínimo 80px de altura) para fácil toque
- **Espaçamento generoso** entre teclas (gap de 0.75rem)
- **Feedback tátil visual** com animação `scale(0.95)` ao toque
- **Display de CPF** com fonte grande e legível (`clamp(1.5rem, 5vh, 2.2rem)`)
- **Sem rolagem** (`overflow: hidden`) para experiência kiosk

### 🔐 Validação de Acesso
- Verificação se o CPF possui exatamente 11 dígitos
- Consulta à API para confirmar cadastro
- Validação do status do aluno (`liberado` / `bloqueado`)
- Mensagens claras de retorno para cada cenário

### 🎨 Experiência Visual
| Status | Cor | Ícone | Mensagem |
|--------|-----|-------|----------|
| Aguardando | Cinza | ⏳ | "Digite os 11 dígitos do seu CPF" |
| Consultando | Roxo | 🔄 | "Verificando cadastro..." |
| Liberado | Verde | ✅ | "ACESSO PERMITIDO - Bom treino!" |
| Bloqueado | Vermelho | ❌ | "ACESSO NEGADO - Procure a recepção" |
| Não Cadastrado | Amarelo | ⚠️ | "CPF NÃO CADASTRADO" |

---

## 📱 Responsividade e Adaptação

| Dispositivo | Comportamento |
|-------------|----------------|
| **Tablet (8"-12")** | Layout ideal, botões no tamanho perfeito para toque |
| **Smartphone** | Adaptação proporcional, mantém usabilidade |
| **Quiosque Touch** | Tela fixa sem rolagem, experiência quiosque completa |
| **Desktop com Mouse** | Botões clicáveis normalmente, sem perda de funcionalidade |

### Variáveis de Altura Dinâmica
```css
height: 100dvh; /* Altura dinâmica para mobile moderno */
max-height: 850px; /* Limite para telas muito grandes */
```

---

## 🗂️ Estrutura do Projeto (Arquivo Único)

```
index.html (Catraca Touch)
├── <head>
│   ├── Meta tags com viewport otimizado (user-scalable=no)
│   ├── TailwindCSS + Font Awesome
│   └── Estilos customizados (glassmorphism, grid-numpad)
├── <body>
│   └── .tablet-container
│       ├── Header (Movement Academy)
│       ├── Display do CPF (com máscara)
│       ├── Grid Numpad (teclado virtual 3x4)
│       │   ├── Dígitos 0-9
│       │   ├── Botão Limpar (🗑️)
│       │   ├── Botão Backspace (⌫)
│       │   └── Botão Validar Acesso (🎫)
│       └── Status Box (feedback do sistema)
└── <script>
    ├── Lógica de digitação e máscara
    ├── Consulta à API
    └── Feedback visual de status
```

---

## 🚀 Como Executar Localmente

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/catraca-touch.git

# Acesse a pasta
cd catraca-touch

# Abra o arquivo em um servidor local (recomendado Live Server)
# Ou simplesmente abra o index.html no navegador
```

> **Para testes em tablet:** Utilize o Chrome DevTools em modo dispositivo ou acesse via rede local.

---

## 📊 Endpoints da API Utilizados

| Método | Rota | Descrição | Autenticação |
|--------|------|-----------|---------------|
| `GET` | `/alunos/:cpf` | Busca aluno pelo CPF | ❌ Não (público para consulta) |

> *A rota de consulta por CPF foi configurada sem autenticação para permitir uso direto no totem.*

### 🔗 API Base URL
```
https://catraca-api.vercel.app
```

### Exemplo de Requisição
```javascript
const response = await fetch(`${API_URL}/alunos/${cpf}`);
const aluno = await response.json();
// Retorno: { nome, cpf, status }
```

---

## 🔧 Possíveis Melhorias Futuras

| Prioridade | Funcionalidade |
|------------|----------------|
| 🔴 Alta | Animação de sucesso/erro com som (feedback auditivo) |
| 🔴 Alta | Reset automático após 5 segundos de inatividade |
| 🟡 Média | Leitura por QR Code (app do aluno) |
| 🟡 Média | Biometria facial para validação |
| 🟢 Baixa | Registro de logs de entrada com timestamp |
| 🟢 Baixa | Exibição do nome do aluno ao validar |

---

## 👥 Créditos e Colaboradores

<div align="center">
  
| Função | Nome | Perfil | Projeto |
|--------|------|--------|---------|
| **🎨 Frontend, UI/UX, Catraca Touch** | [mariajschimidt](https://github.com/mariajschimidt) | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/seu-usuario) | Catraca Touch |
| **⚙️ Backend, API, Banco de Dados** | [fonseca-felix](https://github.com/fonseca-felix) | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/fonseca-felix) | [catraca-api.vercel.app](https://catraca-api.vercel.app) |
| **🖥️ Painel Administrativo** | [mariajschimidt](https://github.com/mariajschimidt) | [![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://projeto-catraca-adm.vercel.app) | Admin Console |

</div>

> *💡 Agradecimento especial ao **fonseca-felix** pela API robusta que alimenta tanto o painel administrativo quanto o sistema de check-in.*

---

## 📄 Licença

Este projeto está sob a licença **MIT**.  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

<p align="center">
  <img src="https://img.shields.io/badge/Made_with-Love-ff69b4.svg" alt="Made with Love" />
  <img src="https://img.shields.io/badge/Touch_Ready-8b5cf6.svg" alt="Touch Ready" />
  <img src="https://img.shields.io/badge/API_by-fonseca--felix-000000.svg" alt="API by fonseca-felix" />
</p>

<p align="center">
  <strong>Feito para agilizar o acesso de alunos à academia.</strong>
</p>

---

## 🔗 Links Rápidos

| Recurso | Link |
|---------|------|
| 🎫 **Catraca Touch** | [projeto-catraca-tablet.vercel.app](https://projeto-catraca-tablet.vercel.app/) |
| 🖥️ **Admin Panel** | [projeto-catraca-adm.vercel.app](https://projeto-catraca-adm.vercel.app) |
| ⚙️ **Backend API** | [catraca-api.vercel.app](https://catraca-api.vercel.app) |
| 👨‍💻 **Backend Developer** | [github.com/fonseca-felix](https://github.com/fonseca-felix) |

---

## 📧 Contato

| Área | Email |
|------|-------|
| 🎨 **Frontend** | maria.prestes.senai@gmail.com |
| ⚙️ **Backend** | felix.fonseca.senai@gmail.com |

---
