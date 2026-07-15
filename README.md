````markdown
# Sistema de Controle de Caixinha por Períodos

Um sistema desenvolvido em **PHP** com armazenamento em **JSON**, criado para controlar a movimentação financeira de equipes técnicas de forma simples, rápida e sem necessidade de banco de dados.

Ideal para empresas que precisam controlar entregas de dinheiro, gastos, saldos por colaborador e prestação de contas entre períodos.

---

# ✨ Principais Recursos

- 🔐 Sistema de login com autenticação
- 👥 Controle de usuários e permissões
- 📅 Controle financeiro por períodos
- 💰 Registro de entregas de dinheiro
- 🧾 Registro de gastos
- 🚇 Cadastro de meios de transporte
- ⚡ Cálculo automático de passagens
- 👨‍🔧 Controle de técnicos
- 📊 Gráficos e estatísticas
- 📈 Comparativo entre períodos
- 📤 Exportação para Excel (CSV)
- 🖨️ Impressão de prestação de contas
- 💾 Backup completo em ZIP
- 🌙 Tema Claro / Escuro
- 📋 Auditoria de alterações
- 📂 Armazenamento em arquivos JSON
- ✅ Compatível com hospedagens compartilhadas

---

# 🚀 Tecnologias

- PHP
- Bootstrap 5
- Chart.js
- JSON

O sistema **não utiliza MySQL nem SQLite**, tornando a instalação extremamente simples.

---

# ✅ Compatibilidade

Compatível com:

- PHP 5.x
- PHP 7.x
- PHP 8.x

Pode ser utilizado em praticamente qualquer hospedagem compartilhada.

---

# 📁 Estrutura

```
index.php
caixinha_dados.json
backup_historico_*.json
```

Todos os dados ficam armazenados em arquivos JSON.

---

# 🔑 Usuário padrão

Na primeira execução o sistema cria automaticamente:

**Usuário**

```
admin
```

**Senha**

```
admin
```

⚠️ Recomenda-se alterar a senha logo após o primeiro acesso.

---

# 👤 Níveis de acesso

## Administrador

Possui acesso completo ao sistema.

Pode:

- Criar usuários
- Excluir usuários
- Criar períodos
- Renomear períodos
- Excluir períodos
- Registrar gastos
- Registrar entregas
- Editar lançamentos
- Excluir lançamentos
- Alterar o valor inicial do caixa
- Cadastrar técnicos
- Excluir técnicos
- Ocultar técnicos dos gráficos
- Cadastrar meios de transporte
- Excluir meios de transporte
- Exportar relatórios
- Gerar backups completos

---

## Visualizador

Pode apenas:

- Consultar informações
- Filtrar registros
- Visualizar gráficos
- Exportar CSV
- Imprimir relatórios
- Alterar sua própria senha

Não possui permissão para modificar os dados do sistema.

---

# 📅 Controle por períodos

Cada período possui seu próprio histórico financeiro.

Ao criar um novo período, o sistema transporta automaticamente os saldos pendentes dos técnicos, evitando perda de informações entre fechamentos.

---

# 💵 Registro de movimentações

Cada lançamento registra:

- Data
- Horário
- Técnico
- Tipo
- Valor
- Observação
- Usuário que criou
- Usuário que editou

Todo o histórico permanece disponível para auditoria.

---

# 🚇 Cálculo automático de transporte

O sistema identifica automaticamente os transportes cadastrados dentro da observação.

Exemplo:

```
Empresa > Cliente (ônibus metrô) > Empresa
```

O valor será calculado automaticamente utilizando os preços cadastrados pelo administrador.

Caso o usuário informe um valor manual, ele também poderá ser utilizado.

---

# 📊 Indicadores financeiros

O painel apresenta automaticamente:

- Caixa do período
- Total gasto
- Total entregue aos técnicos
- Total atualmente com técnicos
- Total para devolução
- Saldo disponível no caixa

Todos os valores são atualizados em tempo real.

---

# 📈 Relatórios

O sistema oferece:

- Impressão da prestação de contas
- Impressão com gráficos
- Exportação para Excel (CSV)
- Comparativo entre períodos
- Evolução histórica dos gastos

---

# 💾 Backup

O botão **Backup ZIP** gera automaticamente um arquivo contendo todos os arquivos JSON do sistema.

Isso permite restaurar completamente o histórico sempre que necessário.

---

# 🔒 Segurança

- Login obrigatório
- Controle de permissões
- Sessões PHP
- Auditoria de usuários
- Alteração individual de senha
- Proteção contra acesso às funções administrativas

---

# 🎯 Objetivo

Este projeto foi desenvolvido para facilitar o controle financeiro de equipes técnicas que recebem dinheiro para despesas operacionais, transporte e deslocamentos.

O foco é oferecer uma solução:

- Simples
- Leve
- Rápida
- Portátil
- Fácil de instalar
- Compatível com hospedagens compartilhadas

Sem depender de banco de dados.

---

# 📄 Licença

Este projeto é disponibilizado gratuitamente.

Caso utilize ou modifique este sistema, os créditos são sempre bem-vindos.

---

## 👨‍💻 Desenvolvedor

**Fernando Ferreira Alves**
````
