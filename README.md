# Zabbix Template Furukawa G2500

> **Requisitos**:
> - Zabbix 6.0+ (compatível também com 7.0)
> - SNMP configurado na OLT
> - Comunidade SNMP padrão: `myisp`

### OBSERVAÇÃO: Desenvolvi o template para meu cenário, confira os filtros, para ajustar ao seu.

### 🌐 Informações gerais:
- Uptime do equipamento
- Uso de CPU
- Uso de memória

### 📈 Monitoramento de portas:
- Tráfego **Rx/Tx** em todas as portas PON
- Tráfego **Rx/Tx** nas portas Uplink
- Estado **administrativo** e **operacional** de cada porta

### 👥 ONU:
- Quantidade total de ONUs conectadas por porta
- Detecção de ONU offline (via triggers)

## 🚨 Triggers incluídas
- CPU alta
- Memória alta
- ONU desconectada
- Porta PON ou Uplink com status down

## 📁 Estrutura do arquivo
O template inclui:
- Descoberta LLD de portas PON
- Descoberta LLD de portas Uplink
- Itens com OIDs SNMP específicos para equipamentos Furukawa
- Triggers e protótipos de trigger automáticos

## 🛠️ Personalização

Caso utilize outra comunidade SNMP, altere no host em:
**Configuration → Hosts → SNMP interfaces**

## 🧑‍💻 Autor
Template desenvolvido por Renan Pablo de Mattos
Contribuições, melhorias e sugestões são bem-vindas.

