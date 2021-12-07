# Filtrando-sem-regex

Aprendemos como filtrar, comparar letra a letra, utilizando expressões regulares, representado pelo fragmento de código abaixo:

    var expressao = new RegExp(this.value,"i");
    if (!expressao.test(nome)) {
        paciente.classList.add("invisivel");
    } else{
        paciente.classList.remove("invisivel");
    }
    
Mas há um modo de fazer essa comparação sem a necessidade de utilizar expressões regulares! Podemos utilizar a função substring, que recebe dois parâmetros, fazendo com que ela devolva parte da string, com o tamanho definido nos parâmetros. O primeiro parâmetro é o início, começando do 0 (que representa o primeiro caractere). O segundo parâmetro define o fim (exclusivo, mostramos até o penúltimo caractere). Por exemplo:

     var string = "Alura";
     var resultado = string.substring(1, 4);
     
     
Extraímos uma string que começa no segundo caractere (número 1) e termina no quarto caractere (número 3, índice anterior ao número 4). O valor da variável resultado é:

    lur
    
Conhecendo essa função, pense em um modo de comparar o valor digitado com parte do nome, sem utilizar expressões regulares. Veja em seguida a resposta do instrutor.
