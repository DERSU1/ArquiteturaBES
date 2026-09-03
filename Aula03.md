# Análise de Estilos Arquiteturais 
---

## 1. Ponto a Ponto (Peer-to-Peer / P2P)

### Conceito e Definição
Neste estilo, não existe uma divisão fixa entre cliente e servidor. Cada nó da rede (chamado de *peer* ou par) atua simultaneamente como cliente e como servidor, podendo requisitar e fornecer recursos, dados ou poder de processamento diretamente para outros nós de forma descentralizada.

### Casos de Uso Comuns
* **Redes de Compartilhamento de Arquivos (Torrents):** Softwares como o BitTorrent, onde os usuários baixam pedaços de arquivos uns dos outros simultaneamente.
* **Criptomoedas e Blockchain:** Redes como o Bitcoin, onde cada nó participante valida e armazena cópias das transações sem depender de um banco central.

### Principais Vantagens
* **Descentralização Extrema:** Elimina completamente o ponto único de falha; mesmo que milhares de nós caiam, a rede continua funcionando se houver nós ativos.
* **Escalabilidade de Carga:** Quanto mais usuários entram na rede, mais recursos (como largura de banda e armazenamento) ela ganha coletivamente.

### Principais Desvantagens
* **Complexidade de Gerenciamento:** É extremamente difícil garantir segurança, consistência de dados e controle de acesso sem uma autoridade central.
* **Desempenho Imprevisível:** Como depende da conexão e disponibilidade de computadores de terceiros (muitas vezes instáveis), a velocidade e a estabilidade variam muito.

---

## 2. Distribuído (Arquitetura Distribuída Descentralizada)

### Conceito e Definição
Embora muitos sistemas modernos usem redes, a arquitetura estritamente **distribuída** foca em rodar componentes de um mesmo sistema lógico em múltiplos computadores fisicamente separados que cooperam trocando mensagens, parecendo ao usuário final como um sistema único. Ela difere do modelo cliente-servidor tradicional por não ter um núcleo centralizado obrigatório, espalhando o processamento de forma homogênea.

### Casos de Uso Comuns
* **Sistemas de Computação em Grid / Computação Científica:** Redes de supercomputadores interligadas para processar simulações climáticas complexas ou cálculos astronômicos massivos (ex: projeto SETI@home).
* **Bancos de Dados Distribuídos Globais:** Sistemas como o Google Spanner, que distribuem dados geograficamente entre múltiplos continentes para garantir baixa latência local.

### Principais Vantagens
* **Tolerância a Falhas Geográficas:** Se um data center inteiro cair por falta de energia ou desastre natural, os nós em outras regiões mantêm o sistema operando.
* **Proximidade com o Usuário (Baixa Latência):** O processamento e os dados podem ser alocados fisicamente mais perto de onde o usuário final está.

### Principais Desvantagens
* **Desafios de Consistência de Dados:** Sincronizar informações em tempo real entre servidores em diferentes partes do mundo é um dos problemas mais complexos da computação (consistência de rede, atrasos de latência).
* **Custo e Complexidade Operacional:** Exige infraestrutura de rede avançada, protocolos complexos de sincronização e equipes altamente especializadas para manutenção.
