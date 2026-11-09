# Staloo — Gestão de Encomendas para Hotelaria

*Staloo* vem de **estalo** — aquele momento em que a solução aparece.  
Nasceu de um problema real na recepção de hotéis: o controle de encomendas feito em papel, sujeito a erros e extravios.

---

## O que é

SaaS B2B para redes hoteleiras. Substitui planilhas e cadernos por um sistema integrado de registro, notificação e retirada de encomendas — com rastreabilidade completa e histórico auditável.

**Piloto ativo:** Quality Suites Long Stay Vila Olímpia — rede Atlântica Hotels, São Paulo/SP.

---

## Funcionalidades

### Recepção
- Registro de encomendas com protocolo automático
- Notificação do morador via WhatsApp
- Confirmação de retirada com assinatura digital
- Busca por nome, protocolo ou unidade habitacional
- Impressão automática de cupom com QR Code (Bematech)

### Gestão
- Dashboard com contadores em tempo real
- Filtros por status: aguardando, retirado, atrasado
- Livros de protocolo com exportação em PDF
- Relatório de movimentação mensal
- Log de atividades auditável

### Administração
- Multi-hotel com isolamento de dados por unidade
- Controle de acesso por papel: admin, gerente, recepção, auditor
- Convites corporativos com primeiro acesso seguro
- Configurações por hotel: nome, fuso horário, notificações

---

## Stack

| Camada | Tecnologia |
|---|---|
| Backend (produção) | Node.js + Express — Railway |
| Backend (V2 staging) | Node.js + Express — Google Cloud Run |
| Autenticação | Firebase Auth + RBAC por papel |
| Banco de dados | Firebase Firestore (isolamento por hotel) |
| Gateway | Cloudflare Access |
| Frontend | HTML/CSS/JS |
| Infraestrutura | GCP · southamerica-east1 |

---

## Status

🟢 **Produção:** piloto ativo com Quality Suites Vila Olímpia  
🔵 **V2:** homologação em andamento — multi-hotel, auth corporativa, deploy privado em Cloud Run

---

Desenvolvido por [Vitor Kauan](https://github.com/vitorkevansart)
