# serverless-framework-AWS-DIO
conceitos de Serverless e Infraestrutura como Código (IaC),  usando o Serverless Framework

O Serverless é um paradigma de computação em nuvem que permite a execução de código sem a necessidade de gerenciar servidores explicitamente. Isso significa que você pode se concentrar na lógica do aplicativo e deixar a infraestrutura para o provedor de nuvem. O Serverless Framework é uma ferramenta popular que ajuda a definir, implantar e gerenciar aplicativos Serverless em várias plataformas de nuvem, como AWS Lambda, Azure Functions, Google Cloud Functions e muitas outras.
A Infraestrutura como Código (IaC) é uma abordagem para gerenciar a infraestrutura de TI de forma programática, usando código.
Em vez de configurar manualmente a infraestrutura, você define a infraestrutura desejada em código, normalmente usando uma linguagem de descrição de infraestrutura,
como YAML ou JSON. Em seguida, você usa ferramentas de automação para provisionar, configurar e gerenciar a infraestrutura com base no código.
Aqui está um exemplo de como você pode usar o Serverless Framework para implementar Serverless e IaC em uma abordagem prática:

01-Instalar o Serverless Framework: Você pode instalar o Serverless Framework globalmente em sua máquina usando npm (gerenciador de pacotes do Node.js) com o seguinte comando:

  npm install -g serverless

02-Configurar as credenciais da nuvem: Depois de instalar o Serverless Framework, você precisa configurar as credenciais da nuvem para a plataforma de nuvem que deseja usar, por exemplo, AWS, Azure ou Google Cloud. Você pode fazer isso executando os comandos de configuração adequados no terminal ou usando variáveis de ambiente.

03-Criar um novo serviço: Você pode criar um novo serviço Serverless usando o comando serverless create com o template que deseja. Por exemplo, para criar um serviço AWS Lambda usando o Node.js, você pode executar o seguinte comando: (css)

  serverless create --template aws-nodejs --path my-service

Isso criará um novo serviço com a estrutura de diretórios e arquivos necessários para começar a desenvolver seu aplicativo Serverless.

04-Definir a configuração do serviço: Dentro do diretório do serviço criado, você encontrará um arquivo chamado serverless.yml, que é o arquivo de configuração do serviço. Neste arquivo, você pode definir a configuração do serviço, como o nome do serviço, o provedor de nuvem, as funções Lambda, os eventos de gatilho, as permissões, as variáveis de ambiente e outras configurações específicas da plataforma de nuvem.

05-Implementar o serviço: Depois de definir a configuração do serviço, você pode implantá-lo na nuvem usando o comando serverless deploy. Isso provisionará automaticamente a infraestrutura necessária na nuvem, como as funções Lambda e os eventos de gatilho, com base na configuração definida no arquivo serverless.yml.

06-Implantação do serviço: Depois de definir sua infraestrutura como código, você pode implantar seu serviço usando o comando deploy do Serverless Framework. Por exemplo, para implantar o serviço na AWS, você pode executar o seguinte comando:

  serverless deploy

