
[PROMPT1]Com base nas fontes fornecidas, faça um resumo dos principais conceitos de segurança, conformidade e identidade abordados na certificação SC-900.

A certificação **SC-900: Segurança da Microsoft, Conformidade e Identidade Fundamentos** aborda conceitos essenciais para a proteção de ambientes em nuvem e locais. Com base nas fontes, o conteúdo está estruturado em quatro grandes pilares:

### 1. Conceitos de Segurança
Esta área foca nos fundamentos teóricos e estratégicos que baseiam as soluções de proteção:
*   **Modelo de Responsabilidade Compartilhada:** Define como as tarefas de segurança são divididas entre o cliente e o provedor de nuvem (Microsoft), variando conforme o ambiente seja local, IaaS, PaaS ou SaaS.
*   **Defesa em Profundidade:** Uma estratégia de segurança em camadas projetada para proteger informações contra acessos não autorizados.
*   **Tríade CIA:** Baseia-se nos princípios de **Confidencialidade, Integridade e Disponibilidade**.
*   **Modelo de Confiança Zero (Zero Trust):** Estratégia que não assume confiança implícita, fundamentada em princípios como "verificar explicitamente", "usar acesso de menor privilégio" e "assumir a violação".
*   **Criptografia e Hash:** Mecanismos para proteger dados em repouso, em trânsito e em uso.

### 2. Conceitos de Identidade e Acesso
A identidade é considerada o novo plano de controle na nuvem, centrada no **Microsoft Entra ID** (anteriormente Azure AD):
*   **Microsoft Entra ID:** Solução de gerenciamento de identidade e acesso baseada em nuvem que conecta usuários a aplicativos, dispositivos e dados.
*   **Tipos de Identidade:** Incluem identidades para usuários, **identidades externas** (via Microsoft Entra External ID) e **identidades de agente** para proteger interações de IA.
*   **Identidade Híbrida:** Integração entre diretórios locais e a nuvem para fornecer uma identidade consistente.

### 3. Soluções de Segurança da Microsoft
O treinamento detalha ferramentas específicas para detecção e resposta a ameaças:
*   **Microsoft Defender XDR:** Proteção unificada em dispositivos (Endpoint), e-mails (Office 365), identidades e aplicativos em nuvem.
*   **Microsoft Sentinel:** Uma solução escalonável de **SIEM** (Gerenciamento de Eventos e Informações de Segurança) e **SOAR** (Orquestração, Automação e Resposta de Segurança).
*   **Microsoft Defender para Nuvem:** Foca no gerenciamento da postura de segurança na nuvem (CSPM) e proteção de carga de trabalho para recursos do Azure e outros ambientes.
*   **Segurança de Infraestrutura do Azure:** Inclui serviços como **Firewall do Azure**, Proteção contra DDoS, Grupos de Segurança de Rede (NSG) e o **Azure Key Vault** para gerenciamento de chaves e segredos.
*   **Microsoft Security Copilot:** Uma solução de IA que se integra ao Sentinel e ao Defender para acelerar a resposta a incidentes e processar prompts de segurança.

### 4. Conceitos de Conformidade e Privacidade
Esta parte foca na governança de dados e no cumprimento de normas regulatórias:
*   **Portal de Confiança do Serviço (Service Trust Portal):** Central de recursos onde a Microsoft compartilha detalhes sobre como cumpre seus compromissos de confiança e conformidade.
*   **Princípios de Privacidade da Microsoft:** Diretrizes que regem como a empresa lida com dados de clientes, incluindo transparência e segurança.
*   **GRC (Governança, Risco e Conformidade):** Envolve conceitos como soberania de dados, residência de dados e privacidade.
*   **Microsoft Purview:** Solução central para gerenciamento de conformidade e governança de dados.
