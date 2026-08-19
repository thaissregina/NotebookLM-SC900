# 📘 Miniguia de Estudos — SC-900

Este miniguia foi desenvolvido com o apoio do NotebookLM a partir das fontes selecionadas para o projeto.

O objetivo é reunir, de forma resumida e estruturada, os principais conceitos abordados na certificação Microsoft Security, Compliance, and Identity Fundamentals (SC-900).

## 📌 Conteúdo

1. Conceitos de Segurança, Conformidade e Identidade
2. Microsoft Entra
3. Soluções de Segurança da Microsoft
4. Soluções de Conformidade da Microsoft

---

## 🔐 1. Conceitos de Segurança, Conformidade e Identidade

Base teórica e metodológica para todas as soluções Microsoft.

*   **Modelo de Responsabilidade Compartilhada:** Define a divisão de tarefas entre o cliente e a Microsoft. A responsabilidade varia conforme o modelo (IaaS, PaaS, SaaS), mas o cliente é **sempre** responsável pelos dados, dispositivos e identidades.
*   **Defesa em Profundidade:** Estratégia que utiliza várias camadas de segurança para proteger os dados. Se uma camada falhar, as outras ainda oferecem proteção.
*   **Tríade CIA:** Princípios de **Confidencialidade** (apenas autorizados acessam), **Integridade** (dados não alterados) e **Disponibilidade** (acesso garantido quando necessário).
*   **Modelo de Confiança Zero (Zero Trust):** Assume que toda tentativa de acesso é uma ameaça. Baseia-se em três princípios: **verificar explicitamente**, **usar acesso de menor privilégio** e **assumir a violação**.
*   **Criptografia e Hash:** A criptografia protege dados em repouso, trânsito e uso; o hash garante que o dado não foi modificado (integridade).

> 💡**Não Confunda:** 
> *   **Criptografia:** Garante que ninguém leia o dado sem a chave (**Confidencialidade**).
> *   **Hash:** Garante que o arquivo é original e não foi alterado (**Integridade**).

---

## 👤 2. Microsoft Entra

Focado no gerenciamento de quem acessa o quê e como.

*   **Microsoft Entra ID:** Serviço de nuvem para gerenciamento de identidades que conecta usuários a aplicativos e dados.
*   **Tipos de Identidade:**
    *   **Identidade Híbrida:** Integração de identidades locais (on-premises) com a nuvem.
    *   **Identidades Externas:** Permite que parceiros ou clientes acessem recursos usando suas próprias credenciais (como Google ou Facebook) via **Microsoft Entra External ID**.
    *   **Identidade de Agente (Agent ID):** Identidade específica para proteger e gerenciar agentes de inteligência artificial.
*   **Recursos de Autenticação e Proteção:** O Entra gerencia processos de autenticação (provar quem você é) e controles de acesso (definir o que você pode acessar).

>💡 **Não Confunda:** 
> *   **Identidade Externa:** Para colaboração com humanos de fora da empresa.
> *   **Identidade de Agente:** Para proteção de identidades usadas por máquinas/IA.

- **Conta de Serviço (Service Principal):** É uma identidade criada para ser utilizada por um aplicativo, serviço ou ferramenta de automação para acessar recursos específicos. O desenvolvedor é responsável por gerenciar e proteger as credenciais (como segredos ou certificados) associadas a essa conta.
- **Identidade Gerenciada (Managed Identity):** É um tipo especial de identidade para recursos do Azure (como Máquinas Virtuais ou Web Apps). A grande vantagem é que ela elimina a necessidade de gerenciar credenciais. O Azure cuida automaticamente da rotação e do armazenamento seguro das chaves no Microsoft Entra ID.

💡**Não confunda:** Na Conta de Serviço, você gerencia o segredo/senha. Na Identidade Gerenciada, o Azure faz todo o gerenciamento de credenciais para você, aumentando a segurança.
---

## 🛡️ 3. Soluções de Segurança da Microsoft

Ferramentas práticas para defesa contra ameaças e proteção de infraestrutura.

*   **Microsoft Defender XDR:** Proteção unificada contra ameaças cibernéticas em dispositivos (Endpoints), e-mails (Office 365), identidades e aplicativos.
*   **Microsoft Sentinel:** Solução nativa de nuvem que combina **SIEM** e **SOAR** para detectar e responder a incidentes em escala organizacional.
*   **Microsoft Defender para Nuvem:** Foca em **CSPM** (Gestão da Postura de Segurança) e proteção de cargas de trabalho no Azure e em ambientes multinuvem.
*   **Segurança de Infraestrutura do Azure:**
    *   **Proteção contra DDoS:** Garante disponibilidade protegendo contra ataques de negação de serviço.
    *   **Firewall do Azure & WAF:** O Firewall protege a rede; o **WAF** protege sites e apps web contra invasões.
    *   **Azure Bastion:** Permite acesso RDP/SSH seguro a VMs sem expô-las com IPs públicos.
    *   **Azure Key Vault:** Armazenamento seguro de chaves de criptografia, segredos e certificados.
*   **Microsoft Security Copilot:** IA que processa prompts para auxiliar analistas de segurança na investigação e resposta rápida a incidentes.

> 💡**Não Confunda:** 
> *   **SIEM (Gerenciamento de Eventos):** Foca em coletar e analisar logs para detectar ameaças.
> *   **SOAR (Resposta e Automação):** Foca em automatizar a reação ao ataque detectado.

---


## 📋 4. Soluções de Conformidade da Microsoft

Governança de dados e transparência sobre como a Microsoft opera.

*   **Microsoft Purview:** Família de soluções para governança de dados e gerenciamento de conformidade. Ajuda a proteger informações confidenciais e a gerenciar riscos de dados.
*   **Portal de Confiança do Serviço (Service Trust Portal):** Central de recursos onde a Microsoft publica relatórios de auditoria independentes e avaliações de risco para provar que seus serviços cumprem normas globais.
*   **Princípios de Privacidade da Microsoft:** Compromissos fundamentais de confiança que garantem que o cliente tem o controle de seus dados e que a Microsoft é transparente sobre o uso deles.
*   **Conceitos de GRC:** Governança, Risco e Conformidade, incluindo a gestão de residência e soberania de dados.

> 💡**Não Confunda:** 
> *   **Purview:** A ferramenta técnica para governar e proteger seus próprios dados.
> *   **Service Trust Portal:** O site para você conferir a conformidade da própria Microsoft.

---
