# Openclaw Skills

Uma coleção de skills reutilizáveis para o **Openclaw**, publicados no **ClawHub**. Cada skill encapsula funcionalidades específicas para automação, monitoramento e gerenciamento remoto.

## 📁 Skills Disponíveis

### 1. **SSH Executor**
Localização: `ssh-executor/`

Executar comandos em hosts remotos via SSH com segurança. Este skill permite:
- Gerenciar conexões SSH usando aliases e configurações locais
- Executar comandos remotos com confirmação para operações destrutivas
- Suportar autenticação baseada em chave privada
- Integração com tmux para workflows baseados em sessões
- Diagnósticos remotos de servidores e estado Linux

**Requisitos:** `ssh`, `bash`, `python3`
**Sistemas Operacionais:** Linux, macOS

**Leia mais:** [ssh-executor/SKILL.md](ssh-executor/SKILL.md)
**ClawHub:** https://clawhub.ai/rickkbarbosa/ssh-executor

---

### 2. **Zabbix Connector**
Localização: `zabbix-connector/`

Monitoramento e interação com a API Zabbix. Este skill permite:
- Consultar alertas ativos e problemas
- Listar hosts, itens e grupos de monitoramento
- Acessar métricas históricas
- Reconhecer eventos e problemas
- Integração segura com Zabbix para operações de leitura e escrita controlada

**Requisitos:** `python3`
**Sistemas Operacionais:** Linux, macOS

**ClawHub:** https://clawhub.ai/rickkbarbosa/zabbix-connector
**Leia mais:** [zabbix-connector/SKILL.md](zabbix-connector/SKILL.md)

---

## 🚀 Como Usar

Cada skill é um pacote independente contendo:
- `SKILL.md` — Documentação detalhada do skill
- `*.skill` — Arquivo de definição do skill para Openclaw
- `release.json` — Metadados e informações de versão
- `scripts/` — Scripts auxiliares para execução
- `references/` — Documentação e guias adicionais

### Instalação
1. Clone ou baixe este repositório
2. Copie o diretório do skill desejado para seu ambiente Openclaw
3. Configure as credenciais e dependências conforme documentado no `SKILL.md` de cada skill

### Publicação no ClawHub
Cada skill neste repositório está pronto para publicação no **ClawHub**. Os arquivos `release.json` e `*.skill.sha256` contêm as informações necessárias para distribuição segura.

---

## 📋 Estrutura do Projeto

```
openclaw-skills/
├── README.md (este arquivo)
├── LICENSE
├── ssh-executor/
│   ├── SKILL.md
│   ├── ssh-executor.skill
│   ├── release.json
│   ├── scripts/
│   └── references/
└── zabbix-connector/
    ├── SKILL.md
    ├── zabbix.skill
    ├── release.json
    ├── scripts/
    └── references/
```

---

## 🔐 Segurança

- **SSH Executor:** Use autenticação baseada em chave privada. Nunca compartilhe chaves privadas via chat ou logs.
- **Zabbix Connector:** Proteja as credenciais de API. Configure um arquivo `.env` local; nunca inclua credenciais reais no repositório.
- Sempre confirme operações destrutivas antes de executá-las.
- Respeite as políticas de chave de host SSH.

---

## 📞 Suporte

Para questões sobre um skill específico, consulte a documentação dentro do diretório do skill:
- [SSH Executor - Regras de Segurança](ssh-executor/SKILL.md#safety-rules)
- [Zabbix Connector - Regras de Segurança](zabbix-connector/SKILL.md#security-rules)

---

## 📜 Licença


---

---

# Openclaw Skills

A collection of reusable skills for **Openclaw**, published on **ClawHub**. Each skill encapsulates specific functionalities for automation, monitoring, and remote management.

## 📁 Available Skills

### 1. **SSH Executor**
Location: `ssh-executor/`

Execute commands on remote hosts over SSH securely. This skill allows you to:
- Manage SSH connections using aliases and local configurations
- Execute remote commands with confirmation for destructive operations
- Support private key-based authentication
- Integration with tmux for session-based workflows
- Remote diagnostics of servers and Linux state

**Requirements:** `ssh`, `bash`, `python3`
**Operating Systems:** Linux, macOS

**Learn more:** [ssh-executor/SKILL.md](ssh-executor/SKILL.md)
**ClawHub:** https://clawhub.ai/rickkbarbosa/ssh-executor

---

### 2. **Zabbix Connector**
Location: `zabbix-connector/`

Monitor and interact with the Zabbix API. This skill allows you to:
- Query active alerts and problems
- List hosts, items, and monitoring groups
- Access historical metrics
- Acknowledge events and problems
- Secure integration with Zabbix for controlled read and write operations

**Requirements:** `python3`
**Operating Systems:** Linux, macOS

**Learn more:** [zabbix-connector/SKILL.md](zabbix-connector/SKILL.md)
**ClawHub:** https://clawhub.ai/rickkbarbosa/zabbix-connector

---

## 🚀 How to Use

Each skill is an independent package containing:
- `SKILL.md` — Detailed skill documentation
- `*.skill` — Skill definition file for Openclaw
- `release.json` — Metadata and version information
- `scripts/` — Helper scripts for execution
- `references/` — Additional documentation and guides

### Installation
1. Clone or download this repository
2. Copy the desired skill directory to your Openclaw environment
3. Configure credentials and dependencies as documented in the `SKILL.md` of each skill

### Publication on ClawHub
Each skill in this repository is ready for publication on **ClawHub**. The `release.json` and `*.skill.sha256` files contain the necessary information for secure distribution.

---

## 📋 Project Structure

```
openclaw-skills/
├── README.md (this file)
├── LICENSE
├── ssh-executor/
│   ├── SKILL.md
│   ├── ssh-executor.skill
│   ├── release.json
│   ├── scripts/
│   └── references/
└── zabbix-connector/
    ├── SKILL.md
    ├── zabbix.skill
    ├── release.json
    ├── scripts/
    └── references/
```

---

## 🔐 Security

- **SSH Executor:** Use private key-based authentication. Never share private keys via chat or logs.
- **Zabbix Connector:** Protect API credentials. Configure a local `.env` file; never include real credentials in the repository.
- Always confirm destructive operations before executing them.
- Respect SSH host key policies.

---

## 📞 Support

For questions about a specific skill, consult the documentation within the skill directory:
- [SSH Executor - Security Rules](ssh-executor/SKILL.md#safety-rules)
- [Zabbix Connector - Security Rules](zabbix-connector/SKILL.md#security-rules)

---

## 📜 License

See the [LICENSE](LICENSE) file for details about this project's license.
Consulte o arquivo [LICENSE](LICENSE) para detalhes sobre a licença deste projeto.


### Donate

* [Buy me a coffee](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=29JLND674CAGY&currency_code=BRL)