# then-e-catch
Utlizando then() e catch() em Promises
- Um cenário muito comum é que precisemos executar um código assim que a promise for resolvida, e para isso usamos o método .then(). Ele nos permite definir justamente a função “resolve” da promise, ou seja, a função que recebe o resultado como parâmetro e é chamada quando a promise é bem sucedida:

- O mesmo vale para quando uma promise é rejeitada. Para evitarmos o término da aplicação usamos o método .catch() para lidar com a rejeição da promise. Assim como no .then(), definimos o .catch() passando uma função como parâmetro que será justamente a função reject que será chamada em caso de rejeição, ou seja, ela própria tem como parâmetro o motivo da rejeição

- Obs.: repare que encadeamos o .catch() no .then(), pois se não fizermos assim o código ainda resultará em erro. Ao encadearmos o .then() e o .catch() a rejeição da promise acontece da forma correta.

- Por fim, assim como temos o try, catch e finally para tratamento de erros, podemos definir um método .finally() que segue o mesmo princípio, sendo executado quando a promise é finalizada, independente de se foi resolvida ou rejeitada:
- Por fim, assim como temos o try, catch e finally para tratamento de erros, podemos definir um método .finally() que segue o mesmo princípio, sendo executado quando a promise é finalizada, independente de se foi resolvida ou rejeitada: Obs.: repare que nesse caso a função de callback não possui nenhum parâmetro.
