# 🛡️ TesteCML_Cyber_Security

## 📌 Objetivo do Projeto

Este projeto tem como foco a simulação de ataques em ambientes virtualizados usando o Cisco Modeling Labs (CML), com o objetivo de demonstrar a importância de segmentação de rede e uso de firewalls como o ASAv. Através da captura e análise de pacotes, é possível comparar cenários com e sem proteção.

---

## 🧪 Estrutura dos Testes

- **Lab 1 – Sem ASAv (Ambiente vulnerável):**
  - PC1 (atacante) realiza testes contra PC2 (vítima)
  - Ferramentas utilizadas: `ping`, `nmap`, `hping3`, `arp-scan`
  - Captura de pacotes com `tshark`
  - Resultado: ataque bem-sucedido

- **Lab 2 – Com ASAv (Ambiente protegido):**
  - Firewall ASAv entre VLANs
  - Expectativa: bloqueio de tráfego malicioso
  - Captura e comparação dos pacotes

---

## 📂 Organização das Pastas

- `ArquivosWireShark/`: capturas de tráfego (.pcapng)
- `Relatorios/`: documentação técnica dos testes
- `TopologiasCML/`: arquivos `.yaml` das topologias usadas
- `Scripts/`: comandos utilizados nos testes

---

## 📈 Resultados

- Ataques realizados no ambiente sem ASAv foram bem-sucedidos:
  - Comunicação direta entre VLANs
  - Varredura de portas e flood SYN sem bloqueio
  - Captura confirmada via Wireshark

- Relatório técnico disponível em:
  - `Relatorios/AtaqueBemSucedido.txt`

---

## 🔐 Recomendação

Implementar firewalls como ASAv e políticas de segmentação entre VLANs para mitigar riscos e proteger ativos da rede.

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
