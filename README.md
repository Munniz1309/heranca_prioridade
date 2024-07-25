# heranca_prioridade

O código implementa um sistema de gerenciamento de tarefas e recursos usando um código de Protocolo de Herança de Prioridade (Priority Inheritance Protocol) e a Prioridade de Teto (Ceiling Priority). 


Explicação do Código

Função add_task: Adicionou uma nova tarefa à lista de tarefas (tasks) com um identificador, tempo de execução, prioridade inicial, e o tempo de bloqueio. As tarefas são armazenadas em um heap (usando a biblioteca heapq) para garantir que a tarefa com a maior prioridade seja executada primeiro.
Função add_resource: Adiciona um novo recurso à lista de recursos com um identificador e prioridade de teto
Função lock_resource: Permite que uma tarefa bloqueie um recurso. A tarefa é então reordenada na fila de tarefas de acordo com sua nova prioridade.
Função unlock_resources: Libera todos os recursos bloqueados por uma tarefa e restaura a prioridade original da tarefa.
Função execute_tasks: Executa as tarefas até que todas sejam completadas. As tarefas são processadas em ordem de prioridade (a maior prioridade é processada primeiro). Se uma tarefa termina sua execução, seus recursos bloqueados são liberados. Caso contrário, a tarefa é re-adicionada à fila com a prioridade atualizada.

