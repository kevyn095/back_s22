Integração com API

Foi utilizada a Exchangerate-API, acessada por meio do método HTTP GET com o Axios.
A resposta em formato JSON é processada para obter a taxa de câmbio entre duas moedas:

const taxa = data.conversion_rates[target.toUpperCase()];


O sistema retorna informações organizadas — moeda base, moeda alvo, taxa de conversão e fonte dos dados — além de tratar possíveis erros de rede ou moedas inválidas.

Uso de SDK (Conceitual)

A função validarPaisSDK simula o funcionamento de um SDK, que abstrai operações complexas de integração.
Ela retorna o status e o nome do país conforme o código informado.

Os SDKs facilitam o desenvolvimento porque:

Simplificam o uso de serviços externos;

Permitem o reaproveitamento de código confiável;

Reduzem erros e aumentam a segurança da integração.

 Configuração na Nuvem (Conceitual)

Para hospedar o sistema em produção, poderiam ser utilizados:

AWS EC2 – oferece controle total do servidor e alta escalabilidade;

Azure App Service – facilita a implantação de aplicações Node.js;

Google Cloud Run – executa de forma serverless e cobra apenas pelo uso.

Essas plataformas garantem disponibilidade, segurança e escalabilidade ao sistema.
