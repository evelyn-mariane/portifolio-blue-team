#  Portfolio-Blue-Team

Bem-vindo(a) ao meu repositório oficial de projetos práticos e investigações de Segurança da Informação. Este espaço é dedicado a documentar laboratórios reais e análises de incidentes focados exclusivamente em segurança defensiva (Blue Team) e monitoramento de SOC.

Todos os projetos foram desenvolvidos de forma autoral utilizando ferramentas de análise baseadas na web, priorizando a mentalidade analítica e a documentação técnica profissional.

##  Projetos Práticos e Investigações em Segurança

### Análise Técnica de Incidente: Phishing (Caso Mercado Livre)
Investigação manual e triagem de um indicador suspeito coletado na plataforma PhishTank, simulando uma campanha fraudulenta de roubo de credenciais direcionada à marca do Mercado Livre.
*   Indicador de Comprometimento (IoC): https://rodovias-livre.online
*   Ferramentas Utilizadas: VirusTotal (Reputação de URL) e WHOIS (Análise de Domínio).
*   Principais Descobertas: Identificação de táticas de evasão contra ferramentas automáticas (0/93 detecções no VirusTotal) devido ao tempo de vida extremamente recente do domínio (apenas 2 dias de existência no WHOIS).
*   Ações de Defesa Recomendadas: Bloqueio de navegação no perímetro corporativo (Proxy/Firewall), processo de derrubada do site (Takedown) e plano de conscientização de colaboradores.
*    [Acesse o PDF do Relatório de Phishing Aqui](./investigacoes-de-seguranca/Relatorio_de_Analise_de_Phishing.pdf)

---

### Relatório Técnico de Inteligência de Ameaças (Cyber Threat Intelligence)
Análise de Cyber Threat Intelligence (CTI) focada no rastreamento e correlação de dados de comportamento de um endereço de IP malicioso ativo e global.
*   Indicador de Comprometimento (IoC): 185.220.101.5
*   Ferramentas Utilizadas: AbuseIPDB (Triagem de abuso), VirusTotal (Cruzamento de motores) e Cisco Talos Intelligence (Validação de risco global).
*   Principais Descobertas: Confirmação de 100% de confiança de abuso no AbuseIPDB com mais de 5.700 denúncias na Alemanha, 10 detecções ativas no VirusTotal mapeando a infraestrutura como um nó de saída da rede Tor, e classificação máxima de risco como reputação "Poor" (Ruim) no banco de dados da Cisco Talos.
*   Ações de Defesa Recomendadas: Bloqueio perimetral nas regras de Firewall, protocolo de contenção com isolamento físico/lógico de hosts infectados e Threat Hunting retroativo via auditoria de logs.
*    [Acesse o PDF do Relatório de IP Malicioso Aqui](./investigacoes-de-seguranca/Relatorio_Tecnico_de_Inteligencia_de_Ameacas.pdf)

---

##  Tecnologias e Plataformas Utilizadas
*   Sistemas e Escritório: LibreOffice Writer (Documentação e Diagramação de Relatórios Técnicos)
*   Plataformas de CTI & Triagem: VirusTotal, WHOIS Domain Tools, AbuseIPDB, Cisco Talos Intelligence, PhishTank.
*   Habilidades Demonstradas: Resposta a Incidentes, Análise de IoCs, Redação de Relatórios Executivos, Mitigação de Riscos Corporativos, Contenção de Malware.


