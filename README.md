#testando site
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=, initial-scale=1.0">
    <title>Nacionalidade</title>

</head>
<body>
    <h1>-------nacionalidade-----</h1>
    Seu País é: <input type="text" name="pais" id="pais">
    <input type="button" value="verificar" onclick="resultado()">
    <div id="mostra">

    </div>

    <script>
        function resultado() {
            var nasc = window.document.querySelector('input#pais')
            var mostra = window.document.querySelector('div#mostra') 
            var paises = String(nasc.value)
            var paises = paises.toLocaleLowerCase()
            if (paises == 'brasil') {
                mostra.innerHTML += `<P>voce é <strong>brasileiro<strong></P>`
                mostra.innerHTML += `<P>provavemente mora no bairro de aguas lindas</p>`
                mostra.innerHTML += `<P>e se chama diego gayzão</p>`
            }else{
                mostra.innerHTML += `<p>voce é gringo</p>`
            }
            
            
        }
    </script>
</body>
</html>

