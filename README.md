# A aplicação Android e o Ciclo de Vida da Activity

## Integrantes:
 - **Leonardo dos Santos**
 - **Daniele Barbosa**
 - **Celso Gabriel**

   
## O que é uma Activity no Android?
- Activity no android é uma tela com uma interface de usuário, que permite experiências ao usuário e interatividade.
- Podemos citar como exemplo uma tela de e-mail, que pode contar a listagem de e-mails recebidos.

## Fluxograma de um ciclo de vida das Activity

![ciclo](img/ciclo.png)

## Entenda como é Ciclo de Vida de uma Activity
-  O ciclo de vida de uma Activity pode ser considerado como um conjunto de callbacks onde permite que as Activity saibam que seus status estão mudando.
-  Esses callbacks fazem com que a Activity tenha a oportunidade de se comportar de maneira apropriada quando o usuário entra e sai de um aplicativo.
- Sabendo disso, podemos citar como os principais Callbacks e estados que as activity podem existir como sendo:

## onCreate() 
- É um método da classe ACTIVITY, na qual chamamos quando estamos criando uma atividade, sendo assim um dos primeiros métodos a serem execultados no ciclo de vida de uma Activity.
 - Para ultilizar este método primeiro temos que configurar a interface do usuparo, onde é o local que definimos o layoute da atividade, podemos usar o " setContentView() ", após isto iniciamos os componentes da interface do usuário, podemos usar os métodos como " findViewById() ".

   ![onCreate](img/OnCreate.png)

  
 ## onStart()
 - Esse callback é invocado quando a Activity sai do estado de interrompida (onStop()) e volta a ser utilizada.
 - Esse método é executado rapidamente e, finalizada essa etapa, a Activity passa para o próximo estado, em que estará pronta para realizar os processos de interação com quem vai utilizar o aplicativo.
* onResume();
* onPause();
* onStop();
* onRestart();
* onDestroy();

- Todos esses métodos estão implicitos à criação da activity, no entanto podem ser reescritos utilizando a anotação @Override e a chamada ao método principal.

## Created:
Método: 'onCreate()'
- É chamado quando a activity é criada e inicializada.
- É também onde devem ser instanciadas as variavéis a serem utilizadas na activity.
- É definido o ficheiro de layout

 ## Started
  - Método: 'onStart()'
  - Método criado anterior à apresentação da activity para o utilizador.

 ## Resumed
  - Método: 'onResume()'
  - É chamado quando a activity está pronta para ser executada e aguarda a manipulação do utilizador.
  - A activite se mantém até a activity sofrer uma alteração(ser fechada ou retirada do ecrã principal).

  ## Stopped
  - Método: 'onStop()'
  - Neste método devem ser feitas as gravações de dados ou chamada a API enquanto fecho uma activity.

  ## Paused
  - Método: 'onPause()'
  - A activity entra no método onPause ou quando alguma outra activity ou aplicação a substitui como elemento visível mo ecrã
  - É o primeiro estado quando fechamos uma activity.
  - **OBS:** É recomendado que não sejam executados processos pesados como gravação de dados em BD, chamadas a APIs, entre outros.

  ## Destroyed
  - Método: 'onDestroy()'
  - É utilizada quando a activity libera os recursos de memória e assim efetivamente é fechada e deixa de existir.

Cada um desses pontos são importantes pois permitem que você gerencie como sua aplicação se comporta, sem excessão. Acontece que a 'Activity' não é algo totalmente estático durante seu funcionamento, devido ao fluxo de dados, a mesma é submetida a funções (ou métodos) que influenciam em seu funcionamento em determinada etapa. 

O maior proveito que pode-se ser tirado de um ciclo de vida de uma Activity recai sobre o uso devido de cada um dos seus respectivos métodos. Entre os beneficios pode ser citado a opção de salvar e restaurar o estado da Activity, garantindo que os dados não sejam perdidos durante mudanças de configuração ou interações com o usuário e que a aplicação responda de forma dinâmica às interações do usuário, como por exemplo, igual a "pausar um vídeo" quando a Activity própria é pausada. A pessoa estar mais imersa e no controle do funcionamento da lógica de seu código. Vale ressaltar que os métodos do ciclo de vida mencionados não são exclusivos do Kotlin; eles fazem parte da estrutura de desenvolvimento Android e estão presentes em outras linguagens suportadas para Android, como Java.




  
  
