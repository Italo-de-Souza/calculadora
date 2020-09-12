# calculadora
Minha primeira calculadora simples

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora</title>
</head>
<body>

    <center>
        <h1>CALCULADORA</h1>

        <input id="numb1" type="number" style="width: 60px;">

            <select id="sinal">
                <option value="+">+</option>
                <option value="-">-</option>
                <option value="/">/</option>
                <option value="*">*</option>
                <option value="**">Potência</option>
            </select>

        <input id="numb2" type="number" style="width: 60px;">

        <button onclick="calcular()">Calcular</button>
        <br>

        <span id="texto"></span>  <span id="resultado"></span>
    
    </center>

</body>
</html>

<script>

    function calcular(){
        
        var n1 = Number(numb1.value);
        var n2 = Number(numb2.value);

        if (sinal.value == "+") {
            
            texto.innerHTML = 'O resultado da soma é igual a :'
            resultado.innerHTML= (n1) + (n2);
        }
        if (sinal.value == "-")  {

            texto.innerHTML = 'O resultado da subtração é igual a :'           
            resultado.innerHTML = (n1) - (n2);
       
        }
        if (sinal.value == "/")  {
            
            texto.innerHTML = 'O resultado da divisão é igual a :'
            resultado.innerHTML = (n1) / (n2);
      
        }
        if (sinal.value == "*")  {
            
            texto.innerHTML = 'O resultado da multiplicação é igual a :'
            resultado.innerHTML = (n1) * (n2);
        }
        if (sinal.value == "**"){

            texto.innerHTML = 'O resultado da potênca é igual a :'
            resultado.innerHTML = (n1) ** (n2);
        }

    }


</script>


