# Atividade Individual Caixa-Branca---AF
<h1> Nome: Nicolas Beloto Armenio</h1>
<h1>RA: 247563</h1>

<h2>NOTAÇÃO DE GRAFO DE FLUXO</h2>
<h3>CONECTAR BD()</h3>
<img width="380" height="160" alt="image" src="https://github.com/user-attachments/assets/e0691309-58bf-48a1-b9fa-57af158813b3" />
<p>N1 – Cria conexão</p>
<p>N2 – Tenta conectar</p>
<p>N3 – Trata erro</p>
<p>N4 – Retorna conexão</p>

<h2>COMPLEXIDADE CICLOMÁTICA</h2> 
<p></p>Fórmula usada: M = E − N + 2P, onde P = número de componentes conectados (P = 1).</p>

<p>Número de nós (N)</p>
<p>Número de arestas (E)</p>

<p>M = E - N + 2p</p>
<p>M = 4 - 4 + 2.1</p>
<p>M = 2</p>


<h2>CAMINHO BÁSICO</h2>

<p>1) --> 1, 2, 3, 4</p>
<p>2) -->  1, 2, 4</p>

<h2>NOTAÇÃO DE GRAFO DE FLUXO</h2>
<h3>VERIFICAR USUARIO()</h3>
<img width="558" height="269" alt="image" src="https://github.com/user-attachments/assets/524c1e67-3164-4feb-af9a-c8f9809e53be" />

<p>N1 – Cria conexão</p>
<p>N2 – Monta a query</p>
<p>N3 – Tenta executar (try)</p>
<p>N4 – Verifica se usuário existe</p>
<p>N5 – Lê o nome</p>
<p>N6 – Trata erro</p>
<p>N7 – Retorna o resultado</p>

<h2>COMPLEXIDADE CICLOMÁTICA</h2> 
<p></p>Fórmula usada: M = E − N + 2P, onde P = número de componentes conectados (P = 1).</p>

<p>Número de nós (N)</p>
<p>Número de arestas (E)</p>

<p>M = E - N + 2p</p>
<p>M = 8 - 7 + 2</p>
<p>M = 3</p>

<h2>CAMINHO BÁSICO</h2> 

1) --> 1, 2, 3, 6, 7
2) --> 1, 2, 3, 4, 7
3) --> 1, 2, 3, 4, 5, 7
