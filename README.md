# 🛡️ Portfolio-Blue-Team

Bem-vindo(a) ao meu repositório oficial de projetos práticos e investigações de Segurança da Informação. Este espaço é dedicado a documentar laboratórios e análises de incidentes focados exclusivamente em segurança defensiva (Blue Team).

## 📂 investigacoes-de-seguranca

### 🔍 Análise Técnica de Phishing (Caso Mercado Livre)

Este projeto simula a triagem e investigação manual que um Analista de SOC realiza ao identificar um indicador suspeito no ambiente corporativo. A análise foi realizada 100% via navegador com ferramentas web, focando em mentalidade analítica e documentação técnica.

*   **Ameaça Detectada:** Phishing / Credential Harvesting (Roubo de Credenciais).
*   **Marca Alvo Simulada:** Mercado Livre.
*   **Indicador de Comprometimento (IoC) Investigado:** `https://rodovias-livre.online`

 Ferramentas Utilizadas:
*   **VirusTotal:** Para análise de reputação da URL contra múltiplos motores de antivírus.
*   **WHOIS:** Para levantamento de dados de registro e propriedade do domínio suspeito.

Principais Descobertas:
1.  **Evasão de Ferramentas Automáticas:** A URL apresentou **0 detecções entre 93 motores de segurança** no VirusTotal. Isso comprovou que o golpe utiliza uma infraestrutura muito recente (Zero-Day) para burlar assinaturas automáticas tradicionais, exigindo intervenção analítica humana.
2.  **Idade do Domínio:** A consulta no WHOIS revelou que o site falso havia sido criado em **11/10/2026** (apenas 2 dias antes da análise). Por se tratar de uma marca consolidada e antiga (Mercado Livre), a idade do link confirmou o caráter fraudulento do domínio.

 Mitigações Recomendadas no Relatório:
*   **Bloqueio de Link:** Implementação de regra de bloqueio do domínio na rede corporativa (Firewall/Proxy).
*   **Derrubada do Site (Takedown):** Envio de denúncia de abuso para a empresa registradora (GoDaddy) e serviços de navegação segura.
*   **Conscientização:** Disparo de alerta interno para os colaboradores sobre a circulação da campanha falsa.

---

Relatório Completo:
O documento técnico detalhado com as explicações passo a passo e todas as evidências visuais capturadas está disponível na minha pasta de investigações:
👉 **[Acesse o PDF do Relatório Aqui](./investigacoes-de-seguranca/Relatorio_de_Analise_de_Phishing.pdf)**
