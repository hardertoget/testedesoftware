Com os testes fornecidos pelo professor o jest não funciona, mas se comentar tudo e utilizar apenas os testes que fiz, funciona normalmente.
RESULTADO: ERRO NO CÓDIGO ->  A variável taskInput não foi inicializada antes de seu uso no teste. Aqui estão alguns passos para corrigir isso:
FAIL  ./app.test.js
  × Deve adicionar e concluir três tarefas (2 ms)

  ● Deve adicionar e concluir três tarefas

    ReferenceError: taskInput is not defined

      73 |
      74 |     tarefas.forEach(tarefa => {
    > 75 |       taskInput.value = tarefa;
         |       ^
      76 |       addTaskBtn.click();
      77 |     });
      78 |

      at taskInput (app.test.js:75:7)
          at Array.forEach (<anonymous>)
      at Object.forEach (app.test.js:74:13)

Test Suites: 1 failed, 1 total                                                                                                                                                               
Tests:       1 failed, 1 total                                                                                                                                                               
Snapshots:   0 total
Time:        4.217 s
Ran all test suites.


