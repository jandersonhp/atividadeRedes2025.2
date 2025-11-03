# 📑 Atividade de Redes de Computadores – 221025

## Parte 1 - Dimensionamento da Rede LAN

### A) Análise dos Requisitos do Escritório de Contabilidade

Este projeto visa dimensionar uma rede local (LAN) para atender um escritório de contabilidade, respeitando as seguintes premissas:

| Requisito | Detalhamento |
| :--- | :--- |
| **Dimensões do Escritório** | 8 metros (Largura) x 10 metros (Comprimento) com pé direito de 3,5 metros. |
| **Pontos de Rede Cabeada** | 14 pontos para computadores, utilizando **Cabo Categoria 6 (Cat 6)**. |
| **Ponto de Acesso Sem Fio** | 1 Access Point (AP) para suportar, no mínimo, **20 dispositivos**. |
| **Computadores** | 14 unidades com Windows, Office e navegadores. Necessidade de rodar softwares de contabilidade online. |
| **Banda Larga** | Mínimo de **500 Mb/s**. |
| **Impressoras** | 2 impressoras a laser (1 monocromática e 1 colorida). |
| **Total de Pontos de Rede** | **15** (14 Computadores + 1 Access Point). |

---

### B) Tarefas Realizadas

#### a. Listagem de Componentes de Hardware e Software

Abaixo estão listados todos os componentes necessários para a montagem e operação do escritório de contabilidade.

| Tipo | Item | Especificação Detalhada | Qtd. |
| :--- | :--- | :--- | :--- |
| **Hardware - Computadores** | Desktop (Ponto de Usuário) | **Processador:** Intel Core i5 (12ª Gen. ou sup.) / AMD Ryzen 5. **Memória RAM:** 16 GB DDR4. **Armazenamento:** SSD NVMe de 512 GB. **Placa de Rede:** Gigabit Ethernet (10/100/1000 Mbps). **Monitor:** LED 23". | 14 |
| **Hardware - Impressoras** | Impressora Laser Monocromática (P/B) | Tecnologia Laser, velocidade $\ge 30$ ppm, com conexão de rede (cabeada ou Wi-Fi). | 1 |
| | Impressora Laser Colorida | Tecnologia Laser, velocidade $\ge 20$ ppm, com conexão de rede (cabeada ou Wi-Fi). | 1 |
| **Hardware - Rede** | Roteador | Suporte a banda $\ge 500$ Mb/s (Fornecido pela operadora). | 1 |
| | **Switch de Rede** | **16 Portas Gigabit Ethernet** (10/100/1000 Mbps), Desempilhado (Unmanaged/Smart Managed) (15 pontos + 1 uplink). | 1 |
| | **Access Point (AP) Corporativo** | Suporte $\ge 20$ dispositivos, tecnologia Wi-Fi 5 (802.11ac) ou Wi-Fi 6 (802.11ax), Dual Band. | 1 |
| | **Cabeamento de Rede** | Bobina de Cabo Cat 6 U/UTP (100% Cobre, Homologado Anatel). | 1 |
| | **Conectores RJ45** | Macho (Plug) e Fêmea (Keystone) Categoria 6. | 30 |
| | **Patch Panel** | 24 portas Cat 6. | 1 |
| | **Rack de Parede** | 8U ou 10U de profundidade adequada. | 1 |
| | Componentes de Infraestrutura | Keystones Cat 6, Tomadas RJ45, Caixas de Superfície, Patch Cords, Eletrodutos/Calhas. | Vários |
| **Software** | Sistema Operacional | **Windows 11 Pro** (Licença por volume ou OEM). | 14 |
| | Pacote de Produtividade | **Microsoft Office Home & Business 2021** (Licença vitalícia). | 14 |
| | Software de Contabilidade | Acesso via navegador/web. | N/A |

---

#### b. Metragem de Cabo Cat 6 e Número de Conectores RJ45

Os cálculos de metragem e conectores baseiam-se na planta física e no detalhamento do projeto, garantindo a folga (**Slack**) de 2.0 metros por ponto.

**1. Metragem Estimada de Cabo Cat 6**

| Ponto de Destino | Descrição | Metragem por Cabo (m) |
| :--- | :--- | :--- |
| Ponto 1 (C1) ao Ponto 14 (C14) | Computadores | 9.5m a 31.0m (conforme detalhe da imagem) |
| Ponto 15 (AP) | Access Point (Teto Central) | 12.0m |
| **TOTAL** | | **259.0m** |

> **Conclusão da Metragem:** O total de cabo Cat 6 necessário é de **259.0 metros**. Para a compra, será adquirida uma bobina padrão de **305 metros**.

**2. Número de Conectores RJ45**

| Item | Quantidade de Pontos | Conectores por Ponto | Total de Conectores Necessários |
| :--- | :--- | :--- | :--- |
| Computadores | 14 | 2 (Patch Panel + Tomada) | **28** |
| Access Point | 1 | 2 (Patch Panel + Ponto Teto) | **2** |
| **TOTAL** | 15 | | **30 Conectores RJ45 (Keystone/Plug)** |

---

#### c. Realização de 3 Orçamentos

Foram simulados três orçamentos com base em preços de mercado pesquisados para os principais componentes.

| Item | Qtd | Orçamento 1 (R$) | Orçamento 2 (R$) | Orçamento 3 (R$) |
| :--- | :--- | :--- | :--- | :--- |
| **Subtotal Computadores** (14 un) | 14 | 49.000,00 | **45.500,00** | 47.600,00 |
| **Subtotal Impressoras** (2 un) | 2 | 4.900,00 | 4.700,00 | **4.700,00** |
| **Subtotal Rede** (Switch, AP, Cabo, etc.) | Vários | 2.670,00 | **2.275,00** | 2.774,00 |
| **Subtotal Software** (14 licenças) | 14 | 37.800,00 | **36.400,00** | 39.200,00 |
| **TOTAL GERAL (R$)** | | **94.370,00** | **88.875,00** | **94.274,00** |

---

#### d. Planilha de Menor Preço e Investimento Total

O **Orçamento 2** apresentou o menor valor total e foi utilizado como referência para a composição final do investimento, aplicando-se o menor preço por item.

| Item | Especificação | Qtd | Custo Unitário (R$) | Custo Total (R$) |
| :--- | :--- | :--- | :--- | :--- |
| **Hardware - Computadores** | Desktop i5/16GB/512GB NVMe/Monitor 23" | 14 | 3.250,00 | **45.500,00** |
| Impressora Laser P/B | Modelo de menor custo (O2) | 1 | 950,00 | **950,00** |
| Impressora Laser Colorida | Modelo de menor custo (O3) | 1 | 3.500,00 | **3.500,00** |
| Switch 16 Portas Gigabit | Unmanaged (O2) | 1 | 480,00 | **480,00** |
| Access Point Wi-Fi 6 | Corporativo (O2) | 1 | 700,00 | **700,00** |
| Cabo Cat 6 U/UTP (305m) | Bobina (O2) | 1 | 480,00 | **480,00** |
| Conectores RJ45/Keystone Cat 6 | Unidade (O2) | 30 | 4,50 | **135,00** |
| Patch Panel 24 portas Cat 6 | (O2) | 1 | 220,00 | **220,00** |
| Rack de Parede 8U | (O2) | 1 | 350,00 | **350,00** |
| Componentes de Rede Diversos | (Tomadas, Patch Cords, etc.) | Vários | *Incluso no Custo Total* | **462,00** |
| **Software** | Windows 11 Pro (Licença) | 14 | 750,00 | **10.500,00** |
| | Office Home & Business 2021 | 14 | 1.850,00 | **25.900,00** |
| **Subtotal Hardware e Software** | | | | **89.177,00** |
| **Serviços** | Instalação, Configuração e Infraestrutura (Estimativa de 15%) | | | **13.376,55** |
| **TOTAL GERAL DO PROJETO** | | | | **102.553,55** |

---

#### e. Planta Física do Escritório de Contabilidade

A planta física demonstra o *layout* do escritório, a disposição dos 14 computadores (C1 a C14), as 2 impressoras, o Access Point (AP) e a localização do Rack/Switch.

> <img src="./assets/plantaescrit.jpg">

---

#### f. Planta Lógica da Rede

O diagrama lógico representa a conectividade e o fluxo de dados dos equipamentos.

| Componente | Função na Rede | Conectividade |
| :--- | :--- | :--- |
| **Roteador da Operadora** | Gatewa y (Banda Larga) | Conecta-se ao Switch. |
| **Switch Gigabit (16P)** | Distribuição e comutação (Camada 2) | Conecta o Roteador, o Patch Panel, as Impressoras. |
| **Patch Panel (24P)** | Organização e terminação do cabeamento horizontal | Conecta-se ao Switch via Patch Cords. |
| **14 Pontos (C1-C14)** | Acesso de Usuários (LAN) | Cabos Cat 6 $\rightarrow$ Patch Panel $\rightarrow$ Switch. |
| **1 Ponto (AP)** | Acesso de Usuários (WLAN) | Cabo Cat 6 $\rightarrow$ Patch Panel $\rightarrow$ Switch. |
| **Plano de Endereçamento** | Exemplo de sub-rede | Rede: `192.168.1.0/24` $\rightarrow$ Máscara: `255.255.255.0` $\rightarrow$ Gateway: `192.168.1.1` (Roteador/Switch L3). |

**Diagrama de Conexão Lógica:**

$$\text{Internet (500Mb/s)} \rightarrow \text{Roteador (Gateway)} \rightarrow \text{Switch Gigabit} $$
$$\text{Switch Gigabit} \rightarrow \begin{cases} \text{Patch Panel} \rightarrow \text{14 Computadores} \\ \text{Patch Panel} \rightarrow \text{1 Access Point} \\ \text{Switch Gigabit} \rightarrow \text{2 Impressoras} \end{cases}$$

> <img src="./assets/plantalog.jpg">