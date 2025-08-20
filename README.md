# natalia
tentando fazer esse negocio aqui
                <li class="nav-item"><a class="nav-link" href="#galeria">Galeria</a></li>                <li class="nav-item"><a class="nav-link" href="#contato">Contato</a></li>            </ul>            <div id="acessibilidade" class="menu-acessibilidade">                 <button id="botao-acessibilidade" class="btn btn-primary fw-bold rotacao-botao" aria-expanded="false">acessibilidade</button>                <div id="opcoes-acessibilidade" class="opcoes-acessibilidade apresenta-lista">                    <button id="aumentar-fonte" class="btn btn-primary fw-bold" aria-label="Aumentar o tamanho da fonte">A+</button>                    <button id="diminuir-fonte" class="btn btn-primary fw-bold" aria-label="diminuir o tamanho da fonte">A-</button>                    <button id="alterna-contraste" class="btn btn-primary fw-bold" aria-label="Alterna o contraste de cores"> <i class="bi bi-shadows"></i></button>                         </div>            </div>                    </nav>    </header>@@ -46,15 +39,15 @@ <h1 class="display-4 text-white fst-italic fw-bold">Boas-vindas a</h1>                        class="btn btn-primary btn-lg botao-inicio fw-semibold">Quero                        conhecer!</a>                </div>                <img src="img/lossy-page1-640px-Os_Mutantes.tif (1).png" alt="A imagem apresenta o grupo musical Os mutantes, sao tres pessoas cantando em um microfone" title="Os mutantes - CC0 Domínio Público / Acervo Arquivo Nacional" class="img-fluid img-inicio">                <img src="img/lossy-page1-640px-Os_Mutantes.tif (1).png" alt="A imagem apresenta o grupo musical Os mutantes, sao tres pessoas cantando em  dois microfones" title="Os mutantes - CC0 Domínio Público / Acervo Arquivo Nacional" class="img-fluid img-inicio">              </div>        </section>        <section id="tropicalia" class="my-5 pt-6 secao-tropicalia" tabindex="0" aria-label="Seção explicativa sobre a tropicália">        <section id="tropicalia" class="my-5 pt-6 secao-tropicalia">            <div class="container d-flex align-items-center ">                <div class="col-4 d-flex justify-content-center fundo-galeria">                    <img src="img/image (1).png" class="rounded-pill" width="273" height="331" loading="lazy">                <div class="col-4 d-flex justify-content-center">                    <img src="img/image (1).png" class="rounded-pill" alt="" width="273" height="331" loading="lazy">                </div>                <div class="col-5">                    <h2>O que foi a Tropicália?</h2>@@ -67,7 +60,7 @@ <h2>O que foi a Tropicália?</h2>            </div>        </section>        <section id="galeria" tabindex="0" aria-label="Seção de galeria de imagens">        <section id="galeria">            <h2 class="text-center pt-5">Galeria</h2>            <div class="container p-3 mt-3 fundo-galeria ">
‎styles.cssCopy file name to clipboardExpand all lines: styles.css-58Lines changed: 0 additions & 58 deletionsOriginal file line numberDiff line numberDiff line change@@ -140,61 +140,3 @@ h2 {.form-control {    background-color: #F1EDEF;}.menu-acessibilidade{    position: fixed;    top:2rem;    right:20px;    z-index: 1000;}.rotacao-botao{    transform: rotate(-90deg);    transform-origin: right center;}.opcoes-acessibilidade{    margin-top:10px;    display: flex;    flex-direction: column;}.opcoes-acessibilidade button{    margin-bottom: 5px;}.apresenta-lista{    display: none;}.alto-contraste{    background-color: var(--alto-contraste-fundo);    color: var(--alto-contraste-texto);}.alto-contraste header,.alto-contraste footer,.alto-contraste .formulario{    background-color: var(--alto-contraste-fundo);    color: var(--alto-contraste-texto);}.alto-contraste .nav-link{    color: var(--alto-contraste-link);}.alto-contraste .botao-inicio,.alto-contraste .formulario button,.alto-contraste .btn-primary{    background-color: var(--alto-contraste-link);    color: var(--alto-contraste-fundo)}.alto-contraste #tropicalia {    background: none;}.alto-contraste #galeria {    background-color: var(--alto-contraste-fundo);}.alto-contraste .fundo-galeria {    background: none;}Collapse commentComment on line R200helipa7 commented on Aug 4, 2025 helipa7on Aug 4, 2025acessibilidadehelipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025
  acessibilidade
  
    A+
    A-
  
helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025
  acessibilidade
  
    A+
    A-
  


[ ]
helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025.menu-acessibilidade{
position: fixed;
top:2rem;
right:20px;
z-index: 1000;
}helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025.rotacao-botao{
transform: rotate(-90deg);
transform-origin: right center;
}helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025.opcoes-acessibilidade{
margin-top:10px;
display: flex;
flex-direction: column;
}helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025.opcoes-acessibilidade button{
margin-bottom: 5px;
}helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025.apresenta-lista{
display: none;
}helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025const botaoDeAcessibilidade = document.getElementById('botao-acessibilidade')
const opcoesDeAcessibilidade = document.getElementById('opcoes-acessibilidade')helipa7 replied on Aug 4, 2025 helipa7on Aug 4, 2025botaoDeAcessibilidade.addEventListener('click', function (){
botaoDeAcessibilidade.classList.toggle('rotacao-botao');
opcoesDeAcessibilidade.classList.toggle('apresenta-lista')
})portobarros-collab replied on Aug 18, 2025 portobarros-collabon Aug 18, 2025//Código omitido

    
    <nav class="container d-flex justify-content-between align-items-center" >
        <img src="img/logo.png" class="nav-img" loading="lazy">
        <ul class="nav mt-5">
            <li class="nav-item"><a class="nav-link" href="#inicio">Início</a></li>
            <li class="nav-item"><a class="nav-link" href="#galeria">Galeria</a></li>
            <li class="nav-item"><a class="nav-link" href="#contato">Contato</a></li>
        </ul>
            <div id="acessibilidade">
                <button id="aumentar-fonte" class="btn btn-primary fw-bold">A+</button>
                <button id="diminuir-fonte" class="btn btn-primary fw-bold">A-</button>
            </div>
    </nav>

    
      
    

      
    

    
  

//Código omitidoportobarros-collab replied on Aug 18, 2025 portobarros-collabon Aug 18, 2025document.addEventListener('DOMContentLoaded', function(){
const aumentaFonteBotao = document.getElementById('aumentar-fonte');
let tamanhoAtualFonte = 1;
aumentaFonteBotao.addEventListener('click', function(){
    tamanhoAtualFonte += 0.1;
    document.body.style.fontSize = `${tamanhoAtualFonte}rem`;

});

    
      
    

      
    

    
  
});meire-2007 replied on Aug 20, 2025 meire-2007on Aug 20, 2025let tamanhoAtualFonte = 1;
aumentaFonteBotao.addEventListener('click', function(){
tamanhoAtualFonte += 0.1;
document.body.style.fontSize = ${tamanhoAtualFonte}rem;
