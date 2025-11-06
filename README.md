# 🤖 Bot de Farm — Sistema Completo para Discord

Um bot avançado para **Discord** desenvolvido com **Discord.js v14**, ideal para servidores que utilizam sistema de **farm (progresso, metas e validação manual)**.  
Permite configurar metas diárias, semanais e mensais, aprovar farms enviados por usuários, e acompanhar rankings automaticamente.

---

## ⚙️ Funcionalidades Principais

- 💰 **Painel Interativo:**  
  Exibe todas as metas ativas (diária, semanal e mensal) com botões de controle direto.

- 📤 **Sistema de Farm:**  
  Usuários podem enviar farms para aprovação com imagem de comprovação.  
  Moderadores podem aprovar ou rejeitar os farms.

- 📈 **Progresso Individual:**  
  Cada usuário pode visualizar seu progresso atual (diário, semanal e mensal) de forma privada via botão.

- 🏆 **Ranking Automático:**  
  Ranking mensal é gerado automaticamente e postado no canal configurado no início de cada mês.

- ⚙️ **Configurações de Metas (Admin):**  
  - Ativar ou desativar metas (diária, semanal, mensal) individualmente.  
  - Editar valores das metas diretamente pelo Discord.  
  - Todas as alterações atualizam o painel em tempo real.

- 🧹 **Limpeza Manual (Admin):**  
  Permite limpar farms diários, semanais ou mensais manualmente com um clique.

- ⏰ **Reset Automático:**  
  - Reset **diário** à meia-noite.  
  - Reset **semanal** toda segunda-feira.  
  - Reset **mensal** no primeiro dia do mês.

---

## 💾 Estrutura de Armazenamento

- `farmData.json` → Armazena os dados de farm dos usuários.  
- `metasConfig.json` → Armazena configurações de metas (ativação e valores).

---

## 🧩 Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)  
- [discord.js v14](https://discord.js.org/)  
- [node-cron](https://www.npmjs.com/package/node-cron)  
- [fs (File System)](https://nodejs.org/api/fs.html)

---

## 🚀 Como Usar

1. **Instale as dependências:**
   ```bash
   npm install discord.js node-cron
Configure o bot:
Abra o arquivo principal (index.js) e configure:


const TOKEN = "SEU_TOKEN_DO_BOT_AQUI";
const ID_CANAL_LOGS = "ID_DO_CANAL_DE_LOGS";
const ID_CARGO_APROVADOR = "ID_DO_CARGO_APROVADOR";
Inicie o bot:


node index.js
Gerar o painel principal:
No Discord, envie:
!painel

👑 Permissões Necessárias
Administradores: Podem alterar metas e limpar farms.

Cargo de aprovador: Pode aprovar/rejeitar farms.

Usuários comuns: Podem registrar farms e visualizar progresso.

📷 Exemplo de Uso
💬 Usuário envia um farm.

📤 Bot encaminha para aprovação.

✅ Moderador aprova → Farm é adicionado ao progresso do usuário.

📈 Painel mostra automaticamente os novos valores.

📌 Observações
Totalmente dinâmico e interativo — atualiza o painel em tempo real.

Pode ser adaptado para sistemas de pontos, XP, produtividade ou gamificação.

Código modular e pronto para personalização.

🔧 Melhorias Futuras
Adicionar ranking diário e semanal.

Sistema de notificações automáticas para metas atingidas.

Suporte a múltiplos servidores (multi-guild).

Desenvolvido com ❤️ e ☕ por [SLandXD].
