Calculadora de soma desenvolvida com HTML, JavaScript e Bootstrap 5 para prática de lógica de programação e manipulação do DOM.


<img width="1162" height="480" alt="{83D1800D-AE2B-458C-A9E5-69ADAE8FDC2B}" src="https://github.com/user-attachments/assets/8d791fb6-ed5f-4307-bb10-418ceeed4e12" />
 Calculadora de Soma

Projeto simples desenvolvido para praticar HTML, JavaScript e Bootstrap 5.

 Tecnologias
- HTML5
- JavaScript
- Bootstrap 5

 Funcionalidades
- Inserção de dois números
- Cálculo automático da soma
- Validação de campos
- Interface responsiva

Objetivo
Praticar manipulação de DOM e lógica de programação.

Codigo
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Calculadora - Soma</title>

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light">

<div class="container mt-5">
    <div class="row justify-content-center">
        <div class="col-md-6">

            <div class="card shadow">
                <div class="card-body">
                    <h3 class="text-center mb-4">Calculadora de Soma</h3>

                    <div class="mb-3">
                        <label class="form-label">Primeiro número</label>
                        <input type="number" id="numero1" class="form-control">
                    </div>

                    <div class="mb-3">
                        <label class="form-label">Segundo número</label>
                        <input type="number" id="numero2" class="form-control">
                    </div>

                    <button class="btn btn-primary w-100" onclick="somar()">
                        Calcular
                    </button>

                    <div class="mt-3">
                        <h5 id="resultado" class="text-center"></h5>
                    </div>

                </div>
            </div>

        </div>
    </div>
</div>

<script>
function somar() {
    var numero1 = parseFloat(document.getElementById("numero1").value);
    var numero2 = parseFloat(document.getElementById("numero2").value);

    if (isNaN(numero1) || isNaN(numero2)) {
        document.getElementById("resultado").innerText = "Digite valores válidos.";
        return;
    }

    var resultado = numero1 + numero2;

    document.getElementById("resultado").innerText = 
        "Resultado da soma: " + resultado;
}
</script>

</body>
</html>
