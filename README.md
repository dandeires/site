#index.html
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Meus objetivos do ano</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<section class="conteudo-principal"></section>
<h2 class="titulo-principal">Meus objetivos do ano<span>_</span></h2>
<div class="botoes">
<button class="botao">Emprego</button>
<button class="botao">Passar no vestibular</button>
<button class="botao">Alcançar o gloria no mbl</button>
<button class="botao">Curso de desenho</button>

</div>

</body>
</html>
#style.css
:root{
    --cor-de-fundo: #1E1E1E;
    --verde: #6FFF57;
    --branco: #FFFFFF;
    --botao-ativo: #3A375E;
    --botao-inativo: rgba(58,55,94,0.5);
    --texto-fundo: rgba(58,55,94,0.3);
    
    }
    
    body{
    background-color: var(--cor-de-fundo);
    color: var(--branco);
    font-family: "Chakra Petch", sans-serif;
    
    }
    
    .conteudo-principal{
    
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    max-width: 1200px;
    width: 100%;
    margin: 0 auto;
    }
    
    .titulo-principal{
    
    text-align: left;
    width: 100%;
    font-size: 32px;
    
    }
    
    .titulo-principal span{
    color: var(--verde)
    }
    
    .botao{
    font-family: "Crakra Petch", sans-serif;
    background-color: var(--botao-inativo);
    color: var(--branco);
    display: flex;
    justify-content: center;
    padding: 1em;
    font-size: 18px;
    align-items: center;
    width: 100%;
    border-bottom: 4px solid var(--botao-ativo);
    border-left: 2px solid var(--botao-ativo);
    border-right: 2px solid var(--botao-ativo);
    border-top: none;
    }
    
    .botao:first-child{
    border-radius: 40px 40px 0 0;
    }
    
    .botoes {
    display: block;
    }
    
    @media screen and (min-width: 768px) {
    .botoes{
    display: flex;
    }
    .botao:first-child {
    border-radius: 40px 0 0 0;
    }
    .botao:last-child{
    border-radius: 0 40px 0 0;
    }
    }
    #main.js
    const botoes = document.querySelectorAll(".botao");

for(let i=0;i<botoes.length;i++){
    botoes[i].onclick = function(){

        for(let j=0; j<botoes.length;j++){
            botoes[j].classList.remove( "ativo");

        }


        botoes[i].classList.add( "ativo");
    }
   
}
