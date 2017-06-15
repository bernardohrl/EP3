=====================
Cat-Alog
=====================
Instalação
----------
  |  A instalação do Polymer é simples, primeiro instale o Node Package Manager:
  |    **npm install -g bower**

  |  Depois instale o Polymer CLI:
  |    **npm install -g polymer-cli**

  Pronto, agora já está tudo certo para usar o Polymer!

Contextualização
----------------
  | Polymer é uma tecnologia que possui duas grande vantagens: a primeira é a capacidade de componentização de elementos e a segunda é a facilidade de passar dados entre elementos difernetes do código.
  | No caso deste trabalho, a tecnologia foi escolhida pelo fato de auxiliar na construção de catálogos da maneira apresentada, afinal possui o componente **iron-pages**, o qual é feito para esta funcionalidade.

Hello World
----------------
  |  Primeiramente deve-se executar o comando "**polymer init starter-kit**", onde será gerado uma série de pastas e arquivos básicos para a estruturação da aplicação. Para levantar a aplicação utilize o comando "**polymer serve --open**". Depois crie dentro da pasta src/starter-kit crie um arquivo **hello-world.html**.

  |  O Hello World nesta linguagem é dado pelo seguinte código:

  |  <dom-module id="hello-world">
  |    <template>
  |      Hello World
  |    </template>

  |    <script>
  |      Polymer({
  |        is: "hello-world",
  |      });
  |    </script>
  |  </dom-module>

Implementação
-------------
  |  A primeira parte da implementação contém apenas **imports** dos elementos do polymer. Abaixo temos o **dom module**, que restringe todo o escopo que será usada a linguagem polymer, dentro deste possuímos elementos como o **template** e o **script**.
  |  Dentro do **template**, temos as **iron-pages**, que são um componente responsável por fazer a passagem de **sections**, as sections são as "páginas" onde o conteúdo se encontra.

  |  Dentro destas páginas temos apenas os dados, onde são utilizadas tags vindas do html. No arquivo **style-sheet.css** temos toda estilização do programa.

  |  A div **controls** apresenta botões que ao serem clicados acionam as funções **_goNext()** ou **_goPrev()**, as quais estão implementadas entro do **script**.

  |  Dentro do script além das funções temos a declaração do **Polymer({});**, e dentro desta temos todas a utilização do javascript do componente. Repare a parte que fala **is: 'Cat-alog-app'**, esta possui a função de nomear o componente, e deve estar de acordo com o **dom module**
