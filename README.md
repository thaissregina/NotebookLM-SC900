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

[PROMPT2]Com base exclusivamente nas fontes fornecidas, explique os principais conceitos da certificação SC-900 de forma estruturada. Para cada conceito, apresente: definição, finalidade, um exemplo prático e, quando houver serviços semelhantes, explique as principais diferenças entre eles. Organize o conteúdo pelos quatro domínios da certificação.

A certificação **SC-900: Segurança da Microsoft, Conformidade e Identidade Fundamentos** está estruturada em quatro domínios principais que cobrem desde a teoria básica até as ferramentas específicas da Microsoft.

### Domínio 1: Conceitos de Segurança, Conformidade e Identidade

*   **Modelo de Responsabilidade Compartilhada**
    *   **Definição:** Um framework que divide as tarefas de segurança entre o provedor de nuvem (Microsoft) e o cliente.
    *   **Finalidade:** Garantir que não haja lacunas na proteção, definindo claramente quem é responsável por cada camada (dados, rede, infraestrutura, etc.).
    *   **Exemplo Prático:** Em um ambiente de **SaaS (Software como Serviço)**, como o Microsoft 365, a Microsoft cuida do data center e do software, mas o cliente é responsável por gerenciar quem tem acesso aos arquivos.
    *   **Diferenças:** No **IaaS**, o cliente tem mais controle (e responsabilidade), incluindo o sistema operacional; no **SaaS**, a Microsoft assume a maior parte da carga, exceto dados e identidades.

*   **Modelo de Confiança Zero (Zero Trust)**
    *   **Definição:** Uma estratégia de segurança baseada no princípio de "nunca confiar, sempre verificar".
    *   **Finalidade:** Proteger ambientes modernos que não possuem mais um perímetro físico definido.
    *   **Exemplo Prático:** Exigir que um funcionário realize uma autenticação multifator (MFA) toda vez que acessar um sistema crítico, mesmo que ele esteja dentro do escritório.

*   **Criptografia e Hash**
    *   **Definição:** Mecanismos para proteger a legibilidade e a integridade dos dados.
    *   **Finalidade:** Proteger dados em repouso (armazenados), em trânsito (na rede) e em uso.
    *   **Diferença:** A **criptografia** torna os dados ilegíveis para quem não tem a chave, enquanto o **hash** cria uma "assinatura" única para garantir que o arquivo não foi alterado (integridade).

### Domínio 2: Gestão de Identidade e Acesso (Microsoft Entra)

*   **Microsoft Entra ID**
    *   **Definição:** Solução de gerenciamento de acesso e identidade baseada em nuvem.
    *   **Finalidade:** Conectar pessoas a seus aplicativos, dispositivos e dados com segurança.
    *   **Exemplo Prático:** Um funcionário usa uma única conta corporativa para acessar o e-mail, o SharePoint e aplicativos externos como o Salesforce.

*   **Identidade Híbrida**
    *   **Definição:** Um cenário onde identidades de diretórios locais (on-premises) são sincronizadas com a nuvem.
    *   **Finalidade:** Fornecer uma experiência de login consistente para usuários que utilizam recursos locais e em nuvem.
    *   **Exemplo Prático:** Um usuário usa a mesma senha do computador de sua mesa para acessar recursos no portal do Azure.

*   **Identidades Externas (Microsoft Entra External ID)**
    *   **Definição:** Funcionalidades que permitem a colaboração com pessoas de fora da organização.
    *   **Finalidade:** Permitir que parceiros ou clientes acessem aplicativos corporativos usando suas próprias identidades (como contas do Google ou Microsoft pessoal).
    *   **Diferença:** Enquanto a **Identidade de Agente** protege interações de IA, as **Identidades Externas** focam na interação humana segura entre empresas.

### Domínio 3: Soluções de Segurança da Microsoft

*   **Microsoft Defender XDR**
    *   **Definição:** Uma solução unificada que protege dispositivos, e-mails, identidades e aplicativos.
    *   **Finalidade:** Detectar e correlacionar ameaças em diferentes pontos de ataque de forma automatizada.
    *   **Exemplo Prático:** Se um e-mail com phishing é detectado, o sistema pode bloquear automaticamente o acesso daquela conta em todos os dispositivos da empresa.

*   **Microsoft Sentinel**
    *   **Definição:** Uma solução de **SIEM** (Gerenciamento de Eventos de Segurança) e **SOAR** (Orquestração e Resposta).
    *   **Finalidade:** Coletar dados de toda a empresa para detectar ataques complexos e automatizar a resposta.
    *   **Diferença:** O **SIEM** foca na análise de logs e detecção; o **SOAR** foca na automação da resposta a esses alertas (como rodar um script de bloqueio automaticamente).

*   **Microsoft Security Copilot**
    *   **Definição:** Ferramenta de IA generativa integrada às soluções de segurança.
    *   **Finalidade:** Acelerar a investigação de incidentes e ajudar analistas a entenderem ameaças via linguagem natural.
    *   **Exemplo Prático:** Um analista pergunta ao Copilot: "Resuma o incidente de login suspeito desta manhã", e a IA gera um relatório detalhado.

### Domínio 4: Conformidade e Privacidade da Microsoft

*   **Portal de Confiança do Serviço (Service Trust Portal)**
    *   **Definição:** Uma central de recursos que compartilha como a Microsoft cumpre seus compromissos de confiança.
    *   **Finalidade:** Fornecer transparência e relatórios de auditoria para os clientes.
    *   **Exemplo Prático:** Uma empresa financeira baixa o relatório de conformidade ISO/IEC da Microsoft para apresentar a um órgão regulador.

*   **Microsoft Purview**
    *   **Definição:** Solução para governança de dados e conformidade.
    *   **Finalidade:** Ajudar a gerenciar riscos de dados, proteger informações confidenciais e cumprir leis de privacidade.
    *   **Exemplo Prático:** Classificar automaticamente arquivos que contenham números de cartões de crédito como "Altamente Confidenciais" para impedir o compartilhamento externo.

*   **Princípios de Privacidade da Microsoft**
    *   **Definição:** Diretrizes como controle, transparência e segurança que regem o tratamento de dados pela Microsoft.
    *   **Finalidade:** Garantir que o cliente seja o dono de seus dados e que eles não sejam usados para fins publicitários sem consentimento.
