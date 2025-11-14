# Caixa-Branca---AF

<h2>NOTAÇÃO DE GRAFO DE FLUXO</h2>
<img width="378" height="551" alt="image" src="https://github.com/user-attachments/assets/2c1cc15a-4ecd-4605-bfd2-5d84d4c13871" />
<p>
Nó 1 (Início):
Início da execução do método verificarUsuario(). Declaração das variáveis iniciais.

Nó 2 (ConectarBD):
Chamada do método conectarBD() para tentar estabelecer a conexão com o banco.

Nó 3 (Montagem da SQL):
Montagem da instrução SQL de consulta, concatenando login e senha informados.

Nó 4 (Execução do Try):
Entrada no bloco try, tentativa de criar o Statement e executar executeQuery(sql).

Nó 5 (Exceção / Tratamento de Erro):
Fluxo seguido caso ocorra alguma exceção no bloco try (ex.: conexão nula, erro SQL).

Nó 6 (Decisão – rs.next() = true):
Resultado da execução do SELECT retornou uma linha válida. Usuário encontrado.

Nó 7 (Decisão – rs.next() = false):
O SELECT não retornou nenhum registro. Usuário não encontrado.

Nó 8 (Retorno – false por exceção):
Retorno do método indicando falha, devido a uma exceção ocorrida no processo.

Nó 9 (Retorno – true):
Retorno positivo, indicando que as credenciais existem no banco (usuário autenticado).

Nó 10 (Retorno – false por usuário não encontrado):
Retorno negativo, indicando que a consulta executou normalmente, mas não encontrou o usuário.
</p>
<h2>COMPLEXIDADE CICLOMÁTICA</h2> 
N = 8 | E = 9 | P = 1

M = 9 - 8 + 2 * 1

M = 3 

Complexidade Ciclomática = 2 

<h2>CAMINHO BÁSICO</h2>

Caminho 1 — Conexão OK e usuário encontrado -> 1 → 2 → 3 → 4 → rs.next()==true → return true 

Caminho 2 — Conexão OK e usuário NÃO encontrado -> 1 → 2 → 3 → 4 → rs.next()==false → return false

Caminho 3 — Erro / exceção / NPE -> 1 → 2 (conn=null) → 3 → 4 → exceção → return false

