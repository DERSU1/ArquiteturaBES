# Análise de Estilos Arquiteturais

Análise simplificada de dois estilos arquiteturais: **Cliente-Servidor** e **Publicador/Assinante (Pub/Sub)**.

---

## 1. Cliente-Servidor (Client-Server)

### Conceito e Definição
Separa o sistema em duas partes: o **cliente** (faz a requisição, como um navegador ou app) e o **servidor** (processa o pedido e devolve a resposta). Funciona de forma síncrona e centralizada.

### Casos de Uso Comuns
* **E-commerce:** Um site de compras (como Mercado Livre), onde o usuário busca produtos e o servidor retorna os resultados.
* **Bancos Digitais:** O aplicativo do banco no celular (cliente) consultando o saldo nos servidores da instituição.

### Principais Vantagens
* **Centralização:** Facilita a segurança, manutenções e atualizações em um único lugar (servidor).
* **Organização:** Separa claramente a interface do usuário da regra de negócio e dados.

### Principais Desvantagens
* **Ponto Único de Falha:** Se o servidor cai, ninguém consegue usar o sistema.
* **Gargalo:** Muitas requisições ao mesmo tempo podem sobrecarregar o servidor.

---

## 2. Publicador/Assinante (Pub/Sub)

### Conceito e Definição
Comunicação assíncrona baseada em eventos. O **publicador** envia uma mensagem para um canal (broker), sem saber quem vai ler. Os **assinantes** se inscrevem nesse canal para receber a mensagem automaticamente.

### Casos de Uso Comuns
* **Plataformas de Streaming:** O YouTube avisa que um vídeo novo foi postado, e os serviços de notificação e recomendação processam isso.
* **Internet das Coisas (IoT):** Sensores de temperatura enviam dados para um canal central que alimenta diferentes painéis de monitoramento.

### Principais Vantagens
* **Desacoplamento:** Quem envia não precisa conhecer quem recebe, facilitando alterações futuras.
* **Escalabilidade:** É fácil adicionar novos assinantes sem alterar o código original.

### Principais Desvantagens
* **Complexidade:** Exige ferramentas de mensageria adicionais (ex: RabbitMQ, Kafka).
* **Rastreio Difícil:** Por ser assíncrono, fica mais difícil debugar erros de ponta a ponta.
