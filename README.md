# MediCare v2 - Sistema de Cuidados de Saúde

## 🏥 Sobre o Projeto

O **MediCare v2** é um sistema completo de gerenciamento de cuidados de saúde, desenvolvido para facilitar o acompanhamento de pacientes e familiares. O sistema oferece funcionalidades avançadas para registro de cuidados, gestão de pacientes e acesso familiar.

## ✨ Funcionalidades Principais

- 👥 **Gestão de Pacientes**: Cadastro e acompanhamento completo
- 🏠 **Acesso Familiar**: Portal dedicado para familiares
- 📋 **Registro de Cuidados**: Sistema detalhado de eventos de cuidado
- 📊 **Relatórios**: Dashboards e relatórios personalizados
- 🔐 **Sistema de Autenticação**: Login seguro com diferentes níveis de acesso
- 📱 **Interface Responsiva**: Funciona perfeitamente em dispositivos móveis
- 🔔 **Notificações**: Sistema de alertas e lembretes

## 🚀 Tecnologias Utilizadas

- **Frontend**: React 18 + TypeScript + Vite
- **UI Framework**: Tailwind CSS + shadcn/ui
- **Backend**: Supabase (Database + Auth + Storage)
- **Containerização**: Docker + Docker Compose
- **Deploy**: Coolify
- **Testes**: Jest + Testing Library

## 📦 Instalação e Configuração

### Pré-requisitos

- Node.js 18+ e npm
- Docker e Docker Compose (opcional)
- Conta no Supabase

### Instalação Local

\`\`\`bash
# 1. Clone o repositório
git clone https://github.com/DBN92/MediCarev2.git
cd MediCarev2

# 2. Instale as dependências
npm install

# 3. Configure as variáveis de ambiente
cp .env.example .env
# Edite o arquivo .env com suas configurações do Supabase

# 4. Inicie o servidor de desenvolvimento
npm run dev
\`\`\`

### Usando Docker

\`\`\`bash
# Inicie todos os serviços
docker-compose up -d

# Acesse a aplicação em http://localhost:8080
\`\`\`

## 🔧 Scripts Disponíveis

\`\`\`bash
npm run dev          # Servidor de desenvolvimento
npm run build        # Build para produção
npm run preview      # Preview do build
npm run test         # Executar testes
npm run lint         # Verificar código
npm run type-check   # Verificar tipos TypeScript
\`\`\`

## 📁 Estrutura do Projeto

\`\`\`
src/
├── components/          # Componentes React reutilizáveis
│   ├── ui/             # Componentes de UI (shadcn/ui)
│   ├── Layout.tsx      # Layout principal
│   ├── AppSidebar.tsx  # Barra lateral
│   └── ...
├── pages/              # Páginas da aplicação
│   ├── Dashboard.tsx   # Dashboard principal
│   ├── Patients.tsx    # Gestão de pacientes
│   ├── Care.tsx        # Registro de cuidados
│   └── ...
├── hooks/              # Custom hooks
├── contexts/           # Contextos React
├── integrations/       # Integrações (Supabase)
└── lib/               # Utilitários e configurações
\`\`\`

## 🌐 Deploy

### Produção com Coolify

O projeto está configurado para deploy automático com Coolify usando o arquivo \`coolify.yml\`.

### Deploy Manual

\`\`\`bash
# Build da aplicação
npm run build

# Os arquivos estarão na pasta dist/
\`\`\`

## 🧪 Testes

O projeto inclui diversos arquivos de teste para garantir a qualidade:

- Testes E2E completos
- Testes de fluxo de demo
- Testes de acesso familiar
- Testes de CRUD de pacientes
- Testes de responsividade

\`\`\`bash
# Executar todos os testes
npm run test

# Testes específicos
node test-demo-flow.cjs
node test-family-access.js
node test-patient-crud.js
\`\`\`

## 🔐 Configuração do Supabase

1. Crie um projeto no [Supabase](https://supabase.com)
2. Configure as tabelas usando os scripts SQL na raiz do projeto
3. Atualize as variáveis de ambiente no arquivo \`.env\`

## 📝 Documentação Adicional

- \`TESTE-ACESSO-FAMILIAR.md\` - Guia de testes para acesso familiar
- Scripts SQL na raiz para configuração do banco de dados
- Arquivos HTML de teste para validação de funcionalidades

## �� Contribuição

1. Faça um fork do projeto
2. Crie uma branch para sua feature (\`git checkout -b feature/AmazingFeature\`)
3. Commit suas mudanças (\`git commit -m 'Add some AmazingFeature'\`)
4. Push para a branch (\`git push origin feature/AmazingFeature\`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo \`LICENSE\` para mais detalhes.

## 📞 Suporte

Para suporte e dúvidas, entre em contato através do GitHub Issues.

---

**Desenvolvido com ❤️ para melhorar o cuidado em saúde**
