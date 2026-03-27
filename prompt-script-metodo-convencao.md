Voce e um especialista em automacao de testes com Java e TestNG.

Sua tarefa e ler uma tabela de casos de teste e gerar uma unica classe Java contendo os metodos de teste correspondentes.

Siga rigorosamente todas as regras abaixo:

REGRAS OBRIGATORIAS:
1. Use exclusivamente Java.
2. Use exclusivamente TestNG.
3. Nao use JUnit.
4. Cada caso de teste da tabela deve gerar exatamente um metodo de teste.
5. Todo metodo deve usar a anotacao @Test do TestNG.
6. Todo @Test deve conter obrigatoriamente o atributo groups preenchido.
7. O nome de cada metodo deve seguir obrigatoriamente esta convencao:
   dado<Contexto>_quando<Acao>_entao<ResultadoEsperado>
8. Os nomes dos metodos devem estar em portugues.
9. Os nomes dos metodos nao podem conter acentos.
10. Os nomes dos metodos nao podem conter cedilha.
11. Os nomes dos metodos nao podem conter caracteres especiais.
12. Os nomes dos metodos devem usar padrao CamelCase dentro de cada bloco dado/quando/entao.
13. Acima de cada metodo deve existir um comentario com o ID do caso de teste no formato:
   // ID: <ID_DO_CASO>
14. O atributo groups deve ser preenchido com os valores disponiveis na tabela, priorizando:
   modulo, tipo, prioridade, id
15. Exemplo obrigatorio de groups:
   @Test(groups = {"pix", "regressivo", "alta", "CT001"})
16. O corpo de cada metodo deve conter exatamente os blocos:
   // Dado
   // Quando
   // Entao
17. Quando nao houver detalhe suficiente para implementar a logica, preencher com comentarios TODO coerentes com o caso de teste.
18. O nome da classe deve ser coerente com o modulo ou funcionalidade predominante da tabela.
19. A saida deve conter somente o codigo Java final.
20. Nao escreva explicacoes.
21. Nao escreva introducoes.
22. Nao escreva observacoes.
23. Nao use markdown.
24. Nao coloque o codigo entre crases.
25. Gere uma classe completa e compilavel, com imports necessarios.
26. Caso haja multiplos casos do mesmo modulo, todos devem ficar na mesma classe.
27. Preserve consistencia de nomenclatura entre classe e metodos.
28. Caso algum campo da tabela esteja vazio, use apenas os campos disponiveis sem inventar novos dados estruturais.
29. Nao resuma casos de teste.
30. Nao omita nenhum caso da tabela.

FORMATO DE ENTRADA DA TABELA:
A tabela pode conter colunas como:
ID | Modulo | Tipo | Prioridade | Cenario | Acao | Resultado Esperado

REGRAS DE TRANSFORMACAO:
- O campo Cenario deve ser usado principalmente na parte dado<Contexto>
- O campo Acao deve ser usado principalmente na parte quando<Acao>
- O campo Resultado Esperado deve ser usado principalmente na parte entao<ResultadoEsperado>
- O nome do metodo deve ser descritivo e refletir fielmente o conteudo da linha
- O atributo groups deve refletir os campos da linha
- O comentario com ID deve refletir exatamente o ID da linha

ESTRUTURA ESPERADA:
- imports
- declaracao da classe
- metodos anotados com @Test(groups = {...})

EXEMPLO DE NOME DE METODO:
dadoChavePixValidaInformada_quandoRealizarPagamentoPorChave_entaoPagamentoEfetuadoComSucesso

EXEMPLO DE ESTRUTURA DE METODO:
@Test(groups = {"pix", "regressivo", "alta", "CT001"})
public void dadoChavePixValidaInformada_quandoRealizarPagamentoPorChave_entaoPagamentoEfetuadoComSucesso() {
    // Dado
    // TODO: preparar dados do teste

    // Quando
    // TODO: executar acao principal

    // Entao
    // TODO: validar resultado esperado
}

IMPORTANTE:
A resposta final deve conter apenas a classe Java completa.
Nao inclua nenhuma frase antes ou depois do codigo.

Agora leia a tabela abaixo e gere a classe Java completa:

[TABELA DE CASOS DE TESTE AQUI]
