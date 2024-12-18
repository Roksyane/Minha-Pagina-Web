<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contadores</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
            background-color: rgb(202, 158, 238);
        }
        table {
            width: 60%;
            margin: 20px auto;
            border-collapse: collapse;
            background-color: white;
        }
        th, td {
            padding: 10px;
            text-align: center;
            border: 1px solid #9168f0;
            font-size: 30px;
            color: #b394fc;
        }
        th {
            background-color: #f2f2f2;
            font-size: 30px;
        }
        button {
            font-size: 1.5rem;
            padding: 5px 10px;
            margin: 5px;
            cursor: pointer;
            color: #9168f0;
            background-color: #cab5fa;
        }
        td button {
            font-size: 2rem;
            color: rgb(119, 0, 255);
        }
        h1{
            font-size: 50px;
            color: #f2f2f2;
        }
    </style>
</head>
<body>
    <h1>Contadores</h1>
    
    <table>
        <thead>
            <tr>
                <th>Nome</th>
                <th>Quantidades</th>
                <th>Contadores</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Copos de água</td>
                <td><span id="contador1">0</span></td>
                <td>
                    <button onclick="alterarContador('contador1', 1)">+</button>
                    <button onclick="alterarContador('contador1', -1)">-</button>
                </td>
            </tr>
            <tr>
                <td>Pontos</td>
                <td><span id="contador2">0</span></td>
                <td>
                    <button onclick="alterarContador('contador2', 1)">+</button>
                    <button onclick="alterarContador('contador2', -1)">-</button>
                </td>
            </tr>
            <tr>
                <td>Voltas na quadra</td>
                <td><span id="contador3">0</span></td>
                <td>
                    <button onclick="alterarContador('contador3', 1)">+</button>
                    <button onclick="alterarContador('contador3', -1)">-</button>
                </td>
            </tr>
            <tr>
                <td>Idas ao banheiro</td>
                <td><span id="contador4">0</span></td>
                <td>
                    <button onclick="alterarContador('contador4', 1)">+</button>
                    <button onclick="alterarContador('contador4', -1)">-</button>
                </td>
            </tr>
            <tr>
                <td>Fuscas azuis</td>
                <td><span id="contador5">0</span></td>
                <td>
                    <button onclick="alterarContador('contador5', 1)">+</button>
                    <button onclick="alterarContador('contador5', -1)">-</button>
                </td>
            </tr>
        </tbody>
    </table>

    <script>
        function alterarContador(contadorId, valor) {
            const contador = document.getElementById(contadorId);
            let valorAtual = parseInt(contador.innerText);
            contador.innerText = valorAtual + valor;
        }
    </script>
</body>
</html>


