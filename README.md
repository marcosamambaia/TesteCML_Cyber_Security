# TesteCML_Cyber_Security

Este repositório contém dois laboratórios desenvolvidos no Cisco Modeling Labs (CML) para demonstrar cenários de segurança em redes com e sem firewall.

## 🔐 Lab 1 – Rede com ASAv (Firewall ativo)

- Simula uma rede segmentada com proteção de firewall.
- Utiliza o Cisco ASAv para aplicar regras de filtragem entre VLANs.
- Testes realizados com ferramentas como `ping`, `nmap`, `hping3` e `arp-scan`.
- Resultados mostram bloqueio eficaz de tráfego malicioso.

## ⚠️ Lab 2 – Rede sem ASAv (Vulnerável)

- Simula uma rede sem proteção entre VLANs.
- O roteador permite roteamento direto entre o atacante (PC1) e a vítima (PC2).
- Testes mostram acesso irrestrito, varredura de portas e simulação de ataque DoS.

## 📂 Estrutura do repositório
TesteCML_Cyber_Security/ ├── LabInvasaoComASAv.yaml ├── LabInvasaoSemASAv.yaml ├── relatorios/ │   ├── relatorio_lab1.txt │   ├── relatorio_lab2.txt ├── resultados/ │   ├── nmap_lab1.txt │   ├── nmap_lab2.txt │   ├── hping3_lab2.txt │   └── ping_lab2.txt

## 🧪 Ferramentas utilizadas

- Cisco Modeling Labs (CML)
- Ubuntu 22.04 (PCs simulados)
- Wireshark
- Nmap
- Hping3
- Arp-scan

## 📌 Objetivo

Demonstrar, de forma prática, a importância de firewalls na proteção de redes internas contra ataques de origem local.

## 📄 Licença

Este projeto é de uso acadêmico e livre para fins educacionais.