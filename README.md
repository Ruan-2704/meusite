<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Primeiro Site</title>
    <link rel="stylesheet" href="css/PrimeiroSite.css">
</head>

<body>
    
    <header class="center">
        <h1>Ruan Lucas</h1>
        <h2>Estudante de Programação</h2>
        
    </header>

    <div>
        <nav>
            <ul class="subpaginas">
                <li>
                    <a class="subpagina" href="html/Sobremim.html">Sobre mim</a>
                </li>
                <li>
                    <a class="subpagina" href="html/Projetos.html">Projetos</a>
                </li>
                <li>
                    <a class="subpagina" href="#html/contato" id="link-contato">Contato</a>

                </li>
            </ul>
        </nav>
        
    <div class="textomim">
        <p>
            
            Sou estudante de Análise e Desenvolvimento de Sistemas e sou apaixonado pela área de programação. <br>  
            A forma como APIs, integrações e sistemas são desenvolvidos me fascina, e meu objetivo é me tornar um profissional capaz de criar e 
            integrar soluções inovadoras. <br>  
            <br>  
            Atualmente, estudo Java, HTML e CSS e desenvolvo pequenos projetos para aplicar meus conhecimentos. <br>  
            Este site é um exemplo disso: um projeto simples, mas significativo, pois representa o início da minha trajetória na programação. <br>  
            Aqui, registrarei minha evolução, adicionando novos projetos, experiências adquiridas e tudo que for aprendendo ao longo do caminho. <br>  
            Cada funcionalidade implementada, cada linha de código aprimorada e cada conhecimento adquirido farão parte deste espaço. <br>  
            <br>  
            Se você está vendo esta página agora, saiba que este é apenas o começo! <br>  
            Com o tempo, este projeto será constantemente atualizado, refletindo minha progressão e aperfeiçoamento na área. <br>  
            Minha meta é me especializar no desenvolvimento de sistemas, APIs e integrações, e futuramente, quem sabe, oferecer esses serviços profissionalmente. <br>  
            <br>  
            Fique à vontade para acompanhar essa jornada e ver de perto minha evolução! 


            
        </p>    
    </div>
    
    <footer id="contato">
        
          <a class="nomeredessociais"href="https://github.com/Ruanlucas-2704?tab=repositories" target="_blank" rel="noopener noreferrer">
            <img src="Imagens/githubsvg.svg" alt="Git Hub">
            <p class="textoredessociais">Git Hub</p> 
          </a>
          <a class="nomeredessociais" href="https://www.instagram.com/ruan_lucas2704/" target="_blank" rel="noopener noreferrer">
            <img src="Imagens/instagramsvg.svg" alt="Instagram">
            <p class="textoredessociais">Instagram</p> 
                
          </a>
          <a class="nomeredessociais"href="https://www.linkedin.com/in/ruan-lucas-6a37071b5/" target="_blank" rel="noopener noreferrer">
            <img src="Imagens/linkedinsvg.svg" alt="Linkedin">
            <p class="textoredessociais">Linkedin</p> 
          </a>
          

    </footer>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            document.getElementById("link-contato").addEventListener("click", function(event) {
                event.preventDefault(); // Impede o comportamento padrão do link
    
                // Obtém o footer
                let footer = document.getElementById("contato");
    
                // Adiciona a classe de destaque
                footer.classList.add("footer-highlight");
    
                // Rola suavemente até o footer
                footer.scrollIntoView({ behavior: "smooth", block: "center" });
    
                // Remove a classe de destaque e volta ao normal após 2 segundos
                setTimeout(() => {
                    footer.classList.remove("footer-highlight");
                    footer.classList.add("footer-normal");
    
                    // Remove a classe "footer-normal" depois de um tempo extra (500ms) para evitar bug visual
                    setTimeout(() => {
                        footer.classList.remove("footer-normal");
                    }, 500);
                }, 2000);
            });
        });
    </script>
    
    
    
</body>

</html>
