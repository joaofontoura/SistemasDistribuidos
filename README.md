# SistemasDistribuidos
Repositório de sistemas distribuídos.

1. Percebi que ao alterar as URL's o tempo de espera para o conteúdo aparecer foi maior e mesmo o H2 estando depois da requisição ele aparece antes, junto com o H1 do html.

2. O problema ocorre por que a função resquest() é assícrona e sendo assim não aguarda a finalização da requisição para realizar outra tafera. Como o H2 é a próxima tarefa e está "pronta" ele é mostrado antes da função retornar as respostas da requisição.

3. Adicionei o H2 dentro da função request(); Alterado no código.
