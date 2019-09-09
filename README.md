# desafio9
Desafio Behind The Code


Desafio 09 | Banco do Brasil
Desafio 09 | Banco do Brasil
Para te ajudar
1 - Introdução
2 - Desafio
3 - Pré-requisitos
4 - Primeira etapa
5 - Subindo a Página no OpenShift
6 - Deletar o projeto
Material de apoio
Troubleshooting
License
Para te ajudar
Material de Apoio
Troubleshooting
License
1 - Introdução
O Banco do Brasil, maior banco da América Latina, com destaque em segmentos como agronegócio, infraestrutura, micro e pequenas empresas. O seu maior propósito é estar próximo das pessoas e ajudar a preservar o que é importante para seus clientes, acionistas, funcionários e toda a sociedade. Por esta razão, pensando no pequeno e médio agricultor, que muitas vezes não tem acesso, desconhece ou não tem capacidade financeira para contratar soluções robustas que os auxiliem na gestão e monitoramento de seus processos produtivos, o Banco do Brasil quer desenvolver solução de baixo custo, para que estes proprietários através do controle de temperatura e umidade do solo, possam planejar melhor sistemas de irrigação baseado no tipo do produto, além de sistema de reconhecimento de pragas e qualidade do plantio através de processamento de imagens capturadas com drones.

2 - Desafio
Nesta solução deverá ser usado, kit com microcontrolador com sensor de temperatura ambiente e umidade do solo, Watson IoT Platform para integração e gerenciamento dos sensores / devices, container na plataforma OpenShift para hospedar programa de gerenciamento e controle, desenvolvido em Python com Flask, Watson Studio para desenvolvimento de modelos de aprendizado de máquina profundo, utilizando Jupyter Notebook e Python, Watson Machine Learning para utilização do modelo gerado, e novamente container em OpenShift para expor API em Python com Flask para processar as imagens.


Imagem 1: Arquitetura IOT.


Imagem 2: Arquitetura AI.




3 - Pré-requisitos
Você deverá cumprir os seguintes itens:

Instalar e configurar Python 3.6 ou mais recente;
Instalar e configurar o Postman para testar sua solução;
Ter uma conta no GitHub ou criar uma nova;
Ter Conhecimentos gerais de Tensor Flow, Keras e Numpy;
Ter conhecimentos gerais em Red Hat OpenShift para subir a aplicação;
4 - Primeira etapa
Primeiramente, você deverá criar um novo repositório no GitHub. Abra sua conta no GitHub e clique em Start Project. Dê um nome para seu repositório e selecione a opção Private, para evitar que sua solução seja copiada. Por fim, clique em Create repository.


Imagem 3: Start a Project


Imagem 4: Criação do repositório

Agora, você deverá importar o código deste repositório para o seu. Para isso, clique em Import Code e cole a URL do repositório do desafio 9. Clique em Begin Import e aguarde o processo ser concluído. Quando concluído, volte para seu repositório e veja seu código.

Imagem 5: Novo repositório do gitHub


Imagem 6: Criação do repositório

5 - Subindo a Página no OpenShift
O Openshift é uma plataforma Open Source desenvolvida pela Red Hat utilizada para a orquestração de containers baseada em Kubernetes. Em outras palavras,é uma plataforma que te permite fazer o deploy de suas imagens sem se preocupar com infraestrutura. Atualmente, esta ferramenta também está presente na IBM Cloud.

Para este desafio, será necessário subir sua página no OpenShift na IBM Cloud. Para isso,abra o portal da IBM Cloud e troque sua conta para 1960796 - IBM PoC - Maratona Behind the Code.


Imagem 7: Selecionando a conta

Após selecionada, o dashboard será atualizado, e o recurso "Cluster de Kubernetes" irá aparecer. Clique em Cluster de Kuernetes e então, selecione o d9.


Imagem 8: Dashboard atualizado.


Imagem 9: OpenShift d9

Você será direcionado para o painel do OpenShift na IBM Cloud. Nesta tela você pode obter algumas informações sobre seu cluster. Para prosseguir o processo, clique em Console da Web do OpenShift para ser direcionado ao Web Console do OpenShift. Você também pode abrir o console pelo seguinte link: https://red.ht/desafiofinal


Imagem 10: Painel do OpenShift na IBM Cloud


Imagem 11: Console do OpenSift

Agora, podemos um projeto. Clique em Create Project. Escolha um nome de sua preferência para o projeto e clique em Create


Imagem 12: Criação do projeto


Imagem 13: Overview do projeto

Na página de Overview, clique em Browse Catalog para continuar o deploy da aplicação. Você será direcionado para um catalogo. Procure pela opção "Python" (apenas Python) e selecione esta opção.


Imagem 14: Selecionando o modelo Python

Quando selecionada, clique em next na etapa de Information. Em Configuration dê o nome da sua aplicação. Este nome deverá ser seu id (OBS: Seu novo ID). Em Git Repository, coloque a URL do seu repositório criado após dar o Fork neste repositório. IMPORTANTE: Antes de clicar em next, clique em Advanced Options.


Imagem 15: Nomeando a aplicação


Imagem 16: Advanced Options

Em Advanced Options, clique em Create New Secret e coloque seu usuário e senha do github. O Secret basicamente serve para guardar informações confidênciais em seu container. Dê um nome ao seu secret e clique em create.


Imagem 17: Criando um secret

Para finalizar o processo, clique em Create. Após criado, clique novamente em Overview e procure pela aplicação que você criou. Espere até que fique azul ao lado de pod. Quando isso acontecer, clique na URL ao lado do nome da aplicação e você será direcionado para a página onde terá instruções sobre as próximas etapas necessárias.


Imagem 18: Overview 2

6 - Deletar o projeto
OBS: Esta etapa deve ser seguida apenas se você quiser deletar e criar novamente seu projeto. Caso tenha cometido algum erro e deseje refazer seu deploy, delete seu projeto e crie novamente o projeto e a aplicação. Para deletar seu projeto, clique no logo no canto superior esquerdo do seu console, selecione os três pontos ao lado do projeto que deseja deletar e clique em Delete Project. Digite o nome do projeto na caixa de diálogo e confirme, e ele será marcado para ser deletado. Após isso, basta seguir novamente o processo de criação de projeto.

Material de apoio
Creating a Red Hat OpenShift on IBM Cloud cluster
Watson IOT Plataform - Python
Keras
Tensor Flow
Troubleshooting
O Console da Web do OpenShift não abriu ao clicar na opção?

Resposta: Abra pelo seguinte link: https://red.ht/desafiofinal


Errei ao criar minha aplicação, o que devo fazer? Resposta: Neste caso, delete seu projeto e crie um novamente.

License
Copyright 2019 Maratona Behind the Code

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.