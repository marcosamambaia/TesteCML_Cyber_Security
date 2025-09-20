# Laboratórios CML – Cenários com e sem ASAv

Este repositório contém dois laboratórios desenvolvidos no Cisco Modeling Labs (CML), com foco em testes de invasão e análise de tráfego entre VLANs. Os cenários foram criados para fins **educacionais e éticos**, com objetivo de demonstrar a importância da segmentação e inspeção de pacotes em ambientes corporativos.

## 🎯 Objetivos Didáticos

- Simular ataques entre VLANs em ambiente controlado
- Demonstrar a diferença entre redes **com** e **sem** firewall ASAv
- Validar conectividade, exposição de serviços e captura de tráfego
- Produzir material técnico para ensino, portfólio e vídeos didáticos

## 🧪 Cenários

### 🔹 Laboratório Sem ASAv (`LabInvasaoSemASAv.yaml`)
- PC1 (Atacante): `192.168.20.10` – VLAN 20
- PC2 (Alvo): `192.168.10.10` – VLAN 10
- Comunicação entre VLANs permitida
- SSH acessível ao atacante
- Sem inspeção ou bloqueio de pacotes

### 🔹 Laboratório Com ASAv (`LabInvasaoComASAv.yaml`)
- ASAv configurado entre VLANs
- Políticas de inspeção e bloqueio aplicadas
- Testes demonstram mitigação de ataques

## 📁 Estrutura dos Arquivos
CML-Laboratorios-ASAv/ ├── LabInvasaoSemASAv.yaml ├── LabInvasaoComASAv.yaml ├── netplan/ │   └── PC1.yaml ├── testes/ │   ├── varredura.txt │   └── ssh-tentativa.txt ├── captura/ │   └── ataque.pcap ├── roteiro/ │   └── invasao-intervlan.txt

## 🛠️ Instruções para Importar no CML

1. Abra o Cisco Modeling Labs
2. Vá em **Import Lab**
3. Selecione o arquivo `.yaml` desejado
4. Aguarde a importação e inicie o laboratório
5. Execute os testes conforme descrito nos arquivos de roteiro

## ⚠️ Aviso Ético

Este projeto é exclusivamente para fins educacionais. Nenhuma técnica aqui descrita deve ser utilizada fora de ambientes controlados e autorizados. O autor reforça o compromisso com a ética digital e a cibersegurança responsável.

---
