# 🛡️ TesteCML_Cyber_Security

## 📌 Objetivo do Projeto

Este projeto tem como foco a simulação de ataques em ambientes virtualizados usando o Cisco Modeling Labs (CML), com o objetivo de demonstrar a importância da segmentação de rede e do uso de firewalls como o ASAv. Através da captura e análise de pacotes, é possível comparar cenários com e sem proteção, evidenciando vulnerabilidades e medidas de mitigação.

---

## 🧪 Estrutura dos Testes

### Lab 1 – Sem ASAv (Ambiente vulnerável)

- PC1 (atacante) realiza testes contra PC2 (vítima)
- Ferramentas utilizadas: `ping`, `nmap`, `hping3`, `arp-scan`
- Captura de pacotes com `tshark`
- Resultado: ataque bem-sucedido

### Lab 2 – Com ASAv (Ambiente protegido)

- Firewall ASAv entre VLANs
- Expectativa: bloqueio de tráfego malicioso
- Captura e comparação dos pacotes

---

## 📂 Organização das Pastas
TesteCML_Cyber_Security/ ├── ArquivosWireShark/     # Capturas de tráfego (.pcapng) ├── Relatorios/            # Documentação técnica dos testes ├── TopologiasCML/         # Arquivos .yaml das topologias usadas ├── Scripts/               # Comandos utilizados nos testes └── README.md              # Este arquivo


---

## 📈 Resultados

Ataques realizados no ambiente sem ASAv foram bem-sucedidos:

- Comunicação direta entre VLANs
- Varredura de portas e flood SYN sem bloqueio
- Captura confirmada via Wireshark

Relatório técnico disponível em:

- `Relatorios/AtaqueBemSucedido.txt`

---

## 🔐 Recomendação

Implementar firewalls como o ASAv e políticas de segmentação entre VLANs para mitigar riscos e proteger ativos da rede contra acessos indevidos e tráfego malicioso.

---

## 🛠️ Requisitos

- Cisco Modeling Labs (CML)
- Ubuntu (PC1 atacante)
- Wireshark / Tshark
- Git + GitHub

---

## 👨‍💻 Autor

**Marco Samambaia**  
Projeto desenvolvido como parte de estudos em segurança ofensiva e redes simuladas.

---
