# 📑 Projeto de Redes de Computadores – 221025
## 🌐 Projeto de Rede LAN – Escritório de Contabilidade

Este projeto visa dimensionar, planejar e orçar uma rede local (LAN) para um escritório de contabilidade, considerando infraestrutura de hardware, software, cabeamento e conectividade lógica.

---

## 📝 Informações do Curso

- **Curso:** Análise e Desenvolvimento de Sistemas – Matinal  
- **Disciplina:** Redes de Computadores  
- **Professor:** Fabiano Lopes  
- **Data:** Nov/2025 – 2º Semestre  
- **Integrantes do Grupo:** Janderson Duarte, Gabriel Oliveira, Yago Reis, Caio Dias e Tomás  

---

## 1️⃣ Dimensionamento da Rede LAN

### A) Requisitos do Escritório

| Requisito                  | Detalhamento |
|-----------------------------|-------------|
| Dimensões do Escritório     | 8m (L) × 10m (C), Pé direito: 3,5m |
| Pontos de Rede Cabeada      | 14 pontos para computadores (Cabo Cat 6) |
| Ponto de Acesso Sem Fio     | 1 Access Point para ≥ 20 dispositivos |
| Computadores                | 14 unidades com Windows, Office e navegadores, rodando softwares de contabilidade online |
| Banda Larga                 | ≥ 500 Mb/s |
| Impressoras                 | 1 monocromática + 1 colorida, ambas a laser |
| Total de Pontos de Rede     | 15 (14 computadores + 1 AP) |

---

## 2️⃣ Tarefas Realizadas

### a) Componentes de Hardware e Software

| Tipo          | Item                  | Especificação Detalhada                                              | Qtd. |
|---------------|----------------------|----------------------------------------------------------------------|------|
| **Hardware - Computadores** | Desktop (Ponto de Usuário) | Intel Core i5 (12ª Gen.) / Ryzen 5, RAM 16GB DDR4, SSD NVMe 512GB, Gigabit Ethernet, Monitor 23" | 14 |
| **Hardware - Impressoras**  | Laser Monocromática | Velocidade ≥ 30ppm, rede cabeada/Wi-Fi                               | 1 |
|                               | Laser Colorida      | Velocidade ≥ 20ppm, rede cabeada/Wi-Fi                               | 1 |
| **Hardware - Rede**          | Roteador            | Suporte ≥ 500Mb/s                                                    | 1 |
|                               | Switch Gigabit 16P  | Unmanaged/Smart, conexão a 15 pontos                                  | 1 |
|                               | Access Point Corporativo | Wi-Fi 5/6 Dual Band, ≥ 20 dispositivos                               | 1 |
|                               | Cabo Cat 6 U/UTP    | Bobina 305m, 100% cobre, homologado Anatel                           | 1 |
|                               | Conectores RJ45/Keystone Cat 6 | Macho/Fêmea                                                       | 30 |
|                               | Patch Panel 24P     | Terminação de cabos                                                   | 1 |
|                               | Rack de Parede 8U   | 8U ou 10U, profundidade adequada                                      | 1 |
| **Infraestrutura Diversa**   | Tomadas RJ45, Caixas, Patch Cords, Eletrodutos | Vários | - |
| **Software**                 | Windows 11 Pro      | Licença por volume/OEM                                                | 14 |
|                               | Office Home & Business 2021 | Licença vitalícia                                                 | 14 |
|                               | Software de Contabilidade | Web-based                                                         | N/A |

### b) Cabeamento e Conectores

- Metragem estimada de Cabo Cat 6: **259,0m**  
- Cada ponto inclui folga (Slack) de **2,0m**  
- Bobina padrão adquirida: **305m**  
- Número de conectores RJ45 necessários: **30**  
  - 28 para computadores  
  - 2 para Access Point  

### c) Orçamentos Simulados

| Item          | Qtd | Orçamento 1 (R$) | Orçamento 2 (R$) | Orçamento 3 (R$) |
|---------------|-----|-----------------|-----------------|-----------------|
| Computadores  | 14  | 49.000,00       | 45.500,00       | 47.600,00       |
| Impressoras   | 2   | 4.900,00        | 4.700,00        | 4.700,00        |
| Rede          | Vários | 2.670,00     | 2.275,00        | 2.774,00        |
| Software      | 14  | 37.800,00       | 36.400,00       | 39.200,00       |
| **TOTAL**     |     | 94.370,00       | 88.875,00       | 94.274,00       |

**Orçamento 2 selecionado** por apresentar o menor valor total.

### d) Planilha de Menor Preço e Investimento Total

| Item                       | Especificação                         | Qtd | Custo Unitário (R$) | Custo Total (R$) |
|-----------------------------|--------------------------------------|-----|-------------------|-----------------|
| Hardware - Computadores     | Desktop i5/16GB/512GB NVMe/Monitor 23" | 14  | 3.250,00          | 45.500,00       |
| Impressora Laser P/B        | Modelo O2                             | 1   | 950,00            | 950,00          |
| Impressora Laser Colorida   | Modelo O3                             | 1   | 3.500,00          | 3.500,00        |
| Switch 16P                  | Unmanaged O2                          | 1   | 480,00            | 480,00          |
| Access Point Wi-Fi 6        | Corporativo O2                        | 1   | 700,00            | 700,00          |
| Cabo Cat 6 (305m)           | Bobina O2                             | 1   | 480,00            | 480,00          |
| Conectores RJ45             | Unidade O2                            | 30  | 4,50              | 135,00          |
| Patch Panel 24P             | O2                                    | 1   | 220,00            | 220,00          |
| Rack 8U                     | O2                                    | 1   | 350,00            | 350,00          |
| Diversos (Patch Cords, Tomadas) | Incluso                            | Vários | Incluso        | 462,00          |
| Windows 11 Pro              | Licença                               | 14  | 750,00            | 10.500,00       |
| Office 2021                 | Licença                               | 14  | 1.850,00          | 25.900,00       |
| **Subtotal Hardware/Software** |                                      |     |                   | 89.177,00       |
| Serviços                    | Instalação/Configuração (15%)        |     |                   | 13.376,55       |
| **TOTAL GERAL DO PROJETO**  |                                      |     |                   | 102.553,55      |

### e) Planta Física do Escritório

Layout físico mostrando:  

- 14 computadores (C1–C14)  
- 2 impressoras  
- 1 Access Point  
- Rack/Switch  

### f) Planta Lógica da Rede

| Componente              | Função              | Conectividade                                |
|-------------------------|-------------------|----------------------------------------------|
| Roteador da Operadora    | Gateway / Banda Larga | Conecta-se ao Switch                        |
| Switch Gigabit 16P       | Distribuição LAN    | Conecta Roteador, Patch Panel, Impressoras  |
| Patch Panel 24P           | Terminação de Cabos | Conecta-se ao Switch via Patch Cords       |
| 14 Pontos LAN (C1–C14)   | Usuários LAN        | Cabo Cat 6 → Patch Panel → Switch           |
| 1 Ponto WLAN (AP)         | Usuários Wireless   | Cabo Cat 6 → Patch Panel → Switch           |

**Plano de Endereçamento:**  

- Rede: 192.168.1.0/24  
- Máscara: 255.255.255.0  
- Gateway: 192.168.1.1
