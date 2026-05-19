# CryptoBot

Bot para Discord desenvolvido em JavaScript que consulta preços de criptomoedas por meio da API pública da Binance e atualiza automaticamente uma mensagem em um canal configurado.

O projeto foi criado para praticar integração com APIs externas, automação de tarefas e desenvolvimento de bots para Discord.

## Funcionalidades

- Consulta de preços de múltiplas criptomoedas
- Integração com a API pública da Binance
- Envio de embed formatada no Discord
- Atualização automática da mesma mensagem em intervalos definidos
- Configuração de token e canal por variáveis de ambiente

## Tecnologias utilizadas

- JavaScript
- Node.js
- Discord.js
- API pública da Binance
- Dotenv

## Como o bot funciona

1. O bot inicia e conecta ao Discord.
2. Em intervalos configurados, consulta os preços das criptomoedas.
3. Monta uma embed com os valores atualizados.
4. Envia a embed no canal definido.
5. Nas próximas execuções, edita a mesma mensagem para manter os dados atualizados sem gerar spam.

## Como executar

### Pré-requisitos

- Node.js instalado
- Aplicação criada no Discord Developer Portal
- Token de bot
- ID do canal onde a mensagem será enviada

### Passos

1. Clone o repositório:

```bash
git clone https://github.com/lucassousa-dev/CryptoBot.git
```

2. Acesse a pasta:

```bash
cd CryptoBot
```

3. Instale as dependências:

```bash
npm i
```

4. Crie um arquivo .env com base no .env.example:

```bash
BOT_TOKEN=seu_token_aqui
CHANNEL_ID=id_do_canal_aqui
```

5. Execute o bot::

```bash
node index.js
```

### Variáveis de ambiente

1. BOT_TOKEN - Token de autenticação do bot no Discord

2. CHANNEL_ID - ID do canal que receberá as atualizações

## Aprendizados aplicados

- Consumo de API REST externa
- Uso de async/await
- Manipulação de embeds no Discord
- Automação com execução periódica
- Organização de configurações sensíveis fora do código-fonte

## Possíveis Evoluções

- Comando para escolher criptomoedas monitoradas
- Intervalo de atualização configurável
- Tratamento mais robusto de falhas da API
- Separação do código em módulos
