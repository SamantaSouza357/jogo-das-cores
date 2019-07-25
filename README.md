# JOGO DAS CORES

##linguagens utilizadas
- HTML
- CSS
- JAVASCRIPT

### Ferramentas das Linguagens

- Utilizamos em `CSS` display Flex e propriedades simples de edição 
- Em `JAVASCRIPT`, utilizamos `FOR`,`MATH`,`FUNCTION`.

 **EX:Função Resetar Jogo**
 ~~~
 function verificarFinal(){
    if(quadradinhos[0].style.backgroundColor == quadradinhos[1].style.backgroundColor && quadradinhos[1].style.backgroundColor == quadradinhos[2].style.backgroundColor && quadradinhos[2].style.backgroundColor == quadradinhos[3].style.backgroundColor){
        resposta.innerHTML = "!!! VOCÊ VENCEU !!!";

        for(let quadrado of quadradinhos){
            quadrado.onclick = null;
            quadrado.classList.add("virarQuadradinho");
        }  
    }
    else{
        resposta.innerHTML= "Ainda não foi !!";
    }
}
~~~