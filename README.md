# Projeto Final - Curso de Redes

Este repositório contém o projeto final do curso de redes, realizado no Cisco Packet Tracer. O objetivo do projeto é criar quatro redes distintas e estabelecer comunicação entre elas. As redes são organizadas conforme as diretrizes abaixo:

## Objetivo Final

- Criar 4 redes no Cisco Packet Tracer usando a faixa de endereços IP 192.168.20.0.
- Estabelecer comunicação entre as redes.
- Seguir as configurações específicas para cada rede.

## Configuração das Redes

### Rede Financeiro

- **Endereço IP:** 192.168.20.0/26
- **Gateway:** 192.168.20.1
- **DHCP:** 192.168.20.2
- **Servidor HTTP (financeiro.ada):** 192.168.20.2
- Conteúdo do site: "Financeiro"
- 4 computadores/notebooks utilizando DHCP.

### Rede RH

- **Endereço IP:** 192.168.20.64/26
- **Gateway:** 192.168.20.65
- **DHCP:** 192.168.20.66
- **Servidor HTTP (rh.ada):** 192.168.20.66
- Conteúdo do site: "RH"
- 3 computadores/notebooks utilizando DHCP.
- 1 impressora com IP fixo: 192.168.20.67.

### Rede Tecnologia

- **Endereço IP:** 192.168.20.192/26
- **Gateway:** 192.168.20.193
- **DNS:** 192.168.20.194
- 1 computador com IP fixo: 192.168.20.195
- 1 servidor DNS que resolve os domínios das redes Financeiro e RH.

### Rede Roteadores

- **Endereço IP:** 192.168.20.128/26
- **Roteador 1 Gateway:** 192.168.20.129
- **Roteador 2 Gateway:** 192.168.20.130
- Configuração de rota estática entre os dois roteadores para permitir acesso às demais redes.

### Distribuição de Redes nos Roteadores

- **Roteador 1:**
  - Rede Financeiro
  - Rede RH
  - Rede Roteadores

- **Roteador 2:**
  - Rede Tecnologia
  - Rede Roteadores

## Equipamentos Utilizados

- Roteadores: Router 2911
- Switches: Switches 2960 24TT

## Visão Final

O objetivo final é permitir a comunicação entre os dispositivos da Rede Financeira, RH e Tecnologia. Deve ser possível que um dispositivo da Rede Financeira acesse o site da Rede RH e vice-versa. Todos os DNS devem ser resolvidos pelo servidor DNS da Tecnologia.
