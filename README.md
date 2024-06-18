# Ciclo-de-vida-de-uma-activity

## Integrantes:
-Leonardo dos Santos 
-Daniele Barbosa 
-Celso Gabriel

## Ciclo de vida da activity
- Existem 6 métodos no ciclo de vida de uma activity: onCreate, onStart, onResume, onPause, onStop e onDestroy.
- Todos esses métodos estão implicitos à criação da activity, no entanto podem ser reescritos utilizando a anotação @Override e a chamada ao método principal.

## Created:
Método: 'onCreat()'
- É chamado quando a activity é criada e inicializada.
- É também onde devem ser instanciadas as variavéis a serem utilizadas na activity.
- É definido o ficheiro de layout

 ## Started
  -Método: 'onStart()'
  -Método criado anterior à apresentação da activity para o utilizador.

 ## Resumed
  -Método: 'onResume()'
  -É chamado quando a activity está pronta para ser executada e aguarda a manipulação do utilizador.
  -A activite se mantém até a activity sofrer uma alteração(ser fechada ou retirada do ecrã principal).

  ## Stopped
  Método: 'onStop()'
  -Neste método devem ser feitas as gravações de dados ou chamada a API enquanto fecho uma activity.

  ## Paused
  Método: 'onPause()'
  -A activity entra no método onPause ou quando alguma outra activity ou aplicação a substitui como elemento visível mo ecrã
  -É o primeiro estado quando fechamos uma activity.
  -OBS: É recomendado que não sejam executados processos pesados como gravação de dados em BD, chamadas a APIs, entre outros.

  ## Destroyed
  Método: 'onDestroy()'
  É utilizada quando a activity libera os recursos de memória e assim efetivamente é fechada e deixa de existir.
  
  
