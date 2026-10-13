<div align="center">

# Joel Gomes Silva

### Desenvolvedor Full Stack · Automação de Processos e Integração de Sistemas

Recife, PE — Brasil

[![Email](https://img.shields.io/badge/E--mail-joel.gomes.silva2003%40gmail.com-0A66C2?style=flat-square&logo=maildotru&logoColor=white)](mailto:joel.gomes.silva2003@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-perfil-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/SEU-USUARIO)

</div>

---

## Sobre

Construo sistemas que tiram processos manuais do caminho: APIs, robôs de automação web e
integrações entre plataformas que não foram feitas para conversar entre si.

Meu trabalho atual é o **CrefazON**, uma plataforma de originação de crédito consignado privado
que leva o cliente da primeira mensagem no WhatsApp até a proposta registrada no portal da
financeira sem intervenção humana — atendimento conduzido por IA, dados validados na entrada e
um robô Playwright operando o portal ponta a ponta.

Trabalho o produto inteiro: modelagem de dados, API, automação, frontend operacional e deploy.

---

## Experiência técnica em projetos

### CrefazON — Plataforma de originação de crédito

Automação completa do fluxo de crédito do trabalhador, empréstimo na conta de energia e
refinanciamento veicular.

| Camada | Implementação |
| --- | --- |
| **API** | NestJS + TypeScript, organizada em módulos por domínio: clientes, propostas, documentos, endereços, dados bancários e profissionais |
| **Atendimento** | Bot de WhatsApp integrado à Evolution API e à Meta Cloud API, com webhooks para recebimento de mensagens |
| **IA** | Claude (Anthropic SDK) conduzindo a coleta conversacional, com motor local determinístico como fallback quando a API está indisponível |
| **Validação** | CPF validado por dígito verificador, datas e CEP checados na entrada — antes de qualquer chamada ao portal |
| **Automação web** | Robô Playwright que faz login, simula, seleciona a oferta, envia documentos e acompanha a proposta no portal da financeira |
| **Dados** | Supabase / PostgreSQL, com persistência de estado parcial para retomar atendimentos interrompidos |
| **Operação** | Dashboard próprio com propostas, conversas e logs do robô em tempo real |
| **Deploy** | Docker, publicado no Railway |

**Decisões de engenharia que valem destacar:** a coleta de dados tem dois motores (IA e local)
porque indisponibilidade de API externa não pode derrubar o atendimento; o estado da conversa é
persistido a cada etapa para que uma queda não custe o cliente; e a validação acontece na borda,
não no portal, para não gastar sessão de robô com dado inválido.

### Sistemas de ponto de venda

| Projeto | Escopo |
| --- | --- |
| **JRS PDV** | Sistema de ponto de venda para gestão comercial — vendas, estoque e relatórios |
| **Twist Cream PDV** | PDV de quiosque: atendente, caixa, emissão de NFC-e e ponte de integração com o Pixet |

### Automação de infraestrutura

| Projeto | Escopo |
| --- | --- |
| **[df-office-updates](https://github.com/joelgomes-29/df-office-updates)** | Automação em PowerShell para gestão de atualizações em parque de máquinas Windows |

---

## Stack

**Backend**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)

**Dados**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)

**Automação & Integrações**
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![WhatsApp API](https://img.shields.io/badge/WhatsApp%20API-25D366?style=flat-square&logo=whatsapp&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic%20API-CC785C?style=flat-square&logo=anthropic&logoColor=white)

**Frontend**
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)

**Infraestrutura**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## Contato

A maior parte do meu código está em repositórios privados de produtos em operação.
Posso apresentar arquitetura, trechos de código e demonstração mediante contato.

[![Email](https://img.shields.io/badge/Falar%20comigo-0A66C2?style=for-the-badge&logo=maildotru&logoColor=white)](mailto:joel.gomes.silva2003@gmail.com)

---

<details>
<summary><b>English summary</b></summary>

<br/>

Full stack developer based in Recife, Brazil, focused on process automation and systems
integration. I build the whole product: data modelling, REST APIs, web automation robots,
operational frontends and deployment.

Currently building **CrefazON**, a payroll-loan origination platform that takes a customer from
a first WhatsApp message to a proposal filed in the lender's portal with no human in the loop —
an AI-driven conversational intake, input validated at the edge, and a Playwright robot driving
the portal end to end. Built with NestJS, TypeScript, Supabase/PostgreSQL, Playwright and the
Anthropic API, containerised with Docker and deployed on Railway.

Most of my code lives in private repositories for products in production. Happy to walk through
architecture and code on request — reach me at
[joel.gomes.silva2003@gmail.com](mailto:joel.gomes.silva2003@gmail.com).

</details>
