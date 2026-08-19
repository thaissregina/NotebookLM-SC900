# NotebookLM-SC900

🎯 OBJETIVO

Este projeto faz parte do Bootcamp Bradesco de Cyber, Dados e IA tem como objetivo utilizar o NotebookLM como ferramenta de apoio aos estudos para a certificação Microsoft Security, Compliance, and Identity Fundamentals (SC-900). A partir de fontes oficiais da Microsoft, serão criados resumos, glossários e materiais de revisão para auxiliar na compreensão dos principais conceitos abordados na certificação.

📚 FONTES
1. Microsoft Learn — Conceitos de segurança, conformidade e identidade: https://learn.microsoft.com/pt-br/training/modules/describe-security-concepts-methodologies/
2. Microsoft Learn — Microsoft Entra Identidade, acesso e funções: https://learn.microsoft.com/pt-br/training/modules/explore-basic-services-identity-types/
3. Microsoft Learn — Soluções de segurança Defender, Sentinel e segurança Azure: https://learn.microsoft.com/pt-br/training/paths/describe-capabilities-of-microsoft-security-solutions/
4. Microsoft Learn — Soluções de conformidade: https://learn.microsoft.com/pt-br/training/modules/describe-compliance-management-capabilities-microsoft/
5. Simulado Oficial da Microsoft para SC-900 : https://learn.microsoft.com/pt-br/credentials/certifications/exams/sc-900/practice/assessment?assessmentId=11&assessment-type=practice&wt.mc_id=practiceassessmentslaunch_blog_blog_wwl_xcsa&source=docs

🧠 ENGENHARIA DE PROMPTS

Com base nas fontes fornecidas, faça um resumo dos principais conceitos de segurança, conformidade e identidade abordados na certificação SC-900.

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

