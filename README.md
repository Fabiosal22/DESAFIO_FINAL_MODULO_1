# DESAFIO_FINAL_MODULO_1
🛡️ README – Análise de Segmentação de Rede (Ambiente Simulado)
📌 Objetivo
Avaliar um ambiente de rede simulado com foco em segmentação, exposição de serviços e identificação de riscos operacionais, utilizando ferramentas como Nmap, RustScan, ping, netdiscover e análise manual.

🖥️ Estrutura do Ambiente
Ambiente simulado com Docker Compose

Redes identificadas:

corp_net – Rede principal da empresa

guest_net – Rede para visitantes

infra_net – Rede crítica para serviços internos

🔎 Descobertas Principais
🚨 Falta de segmentação eficaz: Foi possível acessar a corp_net a partir da guest_net.

🔓 Portas abertas sem necessidade em diversos hosts da infra_net.

❌ Ausência de monitoramento entre as redes.

⚠️ Serviços sensíveis expostos: FTP, SMB, LDAP, MySQL, entre outros.

🧪 Metodologia
Coleta ativa de dados com Nmap, RustScan, ping, etc.

Análise de interfaces de rede (ip a)

Geração de inventário de hosts por rede

Scan de portas e análise de serviços e versões

Verificação de segurança em serviços expostos (ex: FTP, LDAP, MySQL)

Organização e backup de dados em .txt

🛠️ Ferramentas Utilizadas
nmap

rustscan

netdiscover

ping

curl

Comandos Linux para inventário e logs

📋 Ações Recomendadas (Plano 80/20)
🧱 Segmentar redes com VLANs e firewalls internos

🔐 Reforçar autenticação e controle de acesso

🚫 Fechar portas desnecessárias

🔄 Atualizar serviços e sistemas

👀 Implementar ferramentas de monitoramento como Zabbix ou Prometheus

📑 Documentar inventário e mudanças

📂 Estrutura de Arquivos Gerados
bash
Copiar
Editar
/inventario/
├── corp_net_ips.txt
├── infra_net_ips.txt
├── guest_net_ips.txt
├── *_ips_hosts.txt
├── scans/
│   ├── rustscan_output.txt
│   └── nmap_services.txt
└── backups/
    └── diagnostico_rede.txt
📌 Conclusão
A análise revelou sérios riscos de segurança causados por falhas na segmentação e exposição desnecessária de serviços. As recomendações propostas visam corrigir essas vulnerabilidades e criar uma base sólida para a segurança da rede.

📚 Referências
Nmap

RustScan

ChatGPT

Google

Pareto – NSW Health
