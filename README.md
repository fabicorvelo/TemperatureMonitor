# Serviço de Monitoramento de Temperatura, Umidade e Luminosidade

O projeto desenvolvido consiste no monitoramento de ambiente para fatores de temperatura, umidade e luminosidade. Para isso foi utilizado o microcontrolador ESP32, e serviços Node-RED, o MongoDB, MQTT - Mosquitto, AWS (Serviço de computação em Nuvem - Ubuntu) e DNS.

## 🚀 Começando

Essas instruções permitirão que você monte o projeto em operação na sua máquina AWS para fins de desenvolvimento e teste.

Consulte **[Dashboard](http://serverdatactd.sytes.net/)** para saber o modelo conceitual do projeto.

### 📋 Pré-requisitos

Inicialmente você precisará criar uma instancia dentro do serviço AWS EC2

```
Instância t2.micro ou t3.micro com sistema operacional Ubuntu 22.04.2 LTS
```

### 🔧 Instalação

Uma série de exemplos passo-a-passo que informam o que você deve executar para ter um ambiente de desenvolvimento em execução.

Diga como essa etapa será:

```
1.	Acesse o console da AWS e clique em "EC2" para abrir o serviço de computação elástica da Amazon.

2.	Clique em "Launch Instance" (Lançar instância) para começar a criar uma nova instância.

3.	Na página "Choose an Amazon Machine Image" (Escolher uma imagem de máquina Amazon), 
selecione "Ubuntu" como o sistema operacional.

4.	Escolha o tipo de instância que deseja criar, e clique em:
"Next: Configure Instance Details" (Próximo: Configurar detalhes da instância).

5.	Configure as opções da instância, como número de instâncias, tamanho da instância, 
rede e outros detalhes.

6.	Clique em "Next: Add Storage" (Próximo: Adicionar armazenamento) para adicionar armazenamento à instância.

7.	Configure o armazenamento para a instância, como o tipo de volume e o tamanho.

8.	Clique em "Next: Add Tags" (Próximo: Adicionar tags) para adicionar tags à instância.

9.	Adicione tags à instância para ajudar a gerenciá-la.

10.	Clique em "Next: Configure Security Group" (Próximo: Configurar grupo de segurança)
para configurar o grupo de segurança da instância.

11.	Configure as regras de segurança para a instância, como as portas que serão abertas para acesso.

12.	Clique em "Review and Launch" (Revisar e lançar) para revisar as configurações da instância.

13.	Revise as configurações da instância e clique em "Launch" (Lançar) para criar a instância.

14.	Na página "Select an existing key pair or create a new key pair" (Selecionar um par de 
chaves existente ou criar um novo par de chaves), escolha um par de chaves existente ou crie um novo.

15.	Clique em "Launch Instances" (Lançar instâncias) para criar a instância.
```

Em seguida instale o Node-RED:

```
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
sudo apt-get install -y nodejs build-essential
sudo npm install -g --unsafe-perm node-red
```

Por fim inicialize o serviço do Node-RED:

```
node-red
node-red-start
```

Termine com um exemplo de como obter dados do sistema ou como usá-los para uma pequena demonstração.

## ⚙️ Executando os testes

Para executar os teste de funcionamento no Node-RED é necessário abrir URL com endereçamento do IP do servidor AWS EC2.

### 🔩 Analise os testes de ponta a ponta

Abra o navegador web de sua preferencia e digite na URL o endereço IP do computador em nuvem

```
http://IP:1880/
```

### ⌨️ E testes de estilo de codificação

Abra o navegador web de sua preferencia e digite na URL o endereço IP do computador em nuvem

```
http://IP:1880/ui/
```

## 🛠️ Construído com

Mencione as ferramentas que você usou para criar seu projeto

* [Node-RED](https://nodered.org/) - O framework web utilizado
* [MongoDB](https://www.mongodb.com/) - O banco de dados utilizado
* [Mosquitto](https://mosquitto.org/) - O serviço Broker MQTT utilizado
* [Duck DNS](https://www.duckdns.org/) - O serviço DNS utilizado

## 🖇️ Colaborando

Por favor, leia o [Licença Creative Commons](https://br.creativecommons.net/licencas/) para obter detalhes sobre o nosso código de conduta e o processo Creative Commons de Atribuição [CC BY].

## 📌 Versão

Nós usamos [Node-RED](https://nodered.org/) para produção de fluxo de programação da dashboard. Para as versões disponíveis, observe as alínea [Executando no AWS EC2 com Ubuntu](https://nodered.org/docs/getting-started/aws). 

## ✒️ Autores

Sugiro que dê o crédito a todas as pessoas que contribuíram para o projeto desde o início até o fim. Reconhecer o esforço e a dedicação de cada um deles é fundamental para mostrar que valoriza a colaboração e o trabalho em equipe. Além disso, isso pode ser uma forma de motivar as pessoas a continuarem se envolvendo em futuros projetos, sabendo que seu trabalho será reconhecido e valorizado.

* **Desenvolvedor** - *Front-End* - [Fabiane Corvêlo de Araújo](https://github.com/fabicorvelo)
* **Desenvolvedor** - *Back-End* - [Gabriel Charlui Correa](https://github.com/GabrielCharlui)

Você também pode ver a lista de todos os [colaboradores](https://github.com/usuario/projeto/colaboradores) que participaram deste projeto.

## 📄 Licença

[![CC BY 4.0][cc-by-shield]][cc-by]

Este trabalho está licenciado sob a 
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

## 🎁 Expressões de gratidão

* Conte a outras pessoas sobre este projeto 📢;
* Convide alguém da equipe para uma cerveja 🍺;
* Um agradecimento publicamente 🫂;
* etc.

---