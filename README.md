<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Treino de Interpretação de Textos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            padding: 20px;
            max-width: 800px;
            margin: auto;
        }
        h1, h2 {
            text-align: center;
            color: #333;
        }
        .day {
            background-color: #fff;
            padding: 20px;
            margin: 20px 0;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        .questions {
            margin-top: 15px;
        }
        .question {
            margin-bottom: 10px;
        }
        .show-answer {
            margin-top: 5px;
            color: #007BFF;
            cursor: pointer;
            font-size: 0.9em;
        }
        .answer {
            display: none;
            margin-top: 5px;
            padding: 10px;
            background-color: #e6f2ff;
            border-left: 4px solid #007BFF;
        }
    </style>
</head>
<body>

    <h1>Treino Diário de Interpretação de Textos</h1>
    <h2>Dia 1</h2>

    <div class="day">
        <p><strong>Texto:</strong> As abelhas desempenham um papel fundamental na polinização das plantas, o que ajuda na produção de alimentos e na manutenção da biodiversidade. Sem elas, muitos ecossistemas sofreriam desequilíbrio.</p>
        
        <div class="questions">
            <div class="question">
                1. Qual é o tema principal do texto? 
                <div class="show-answer" onclick="toggleAnswer(this)">Mostrar resposta</div>
                <div class="answer">O papel das abelhas na polinização e na manutenção dos ecossistemas.</div>
            </div>
            <div class="question">
                2. Por que as abelhas são importantes, segundo o autor? 
                <div class="show-answer" onclick="toggleAnswer(this)">Mostrar resposta</div>
                <div class="answer">Porque ajudam na produção de alimentos e na manutenção da biodiversidade.</div>
            </div>
            <div class="question">
                3. O que aconteceria sem as abelhas? 
                <div class="show-answer" onclick="toggleAnswer(this)">Mostrar resposta</div>
                <div class="answer">Muitos ecossistemas sofreriam desequilíbrio.</div>
            </div>
        </div>
    </div>

    <script>
        function toggleAnswer(el) {
            const answer = el.nextElementSibling;
            if (answer.style.display === "block") {
                answer.style.display = "none";
                el.textContent = "Mostrar resposta";
            } else {
                answer.style.display = "block";
                el.textContent = "Ocultar resposta";
            }
        }
    </script>

</body>
</html>
