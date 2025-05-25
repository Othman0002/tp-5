# tp-5
tp 5
<!DOCTYPE html>
<html>
<head>
<title>Quiz realise pa OThMAN BAHAMMOU</title>
</head>
<body>
<h1>Bienvenue dans mon petit  Quiz !</h1>
<button onclick="lancerQuiz()">Démarrer le Quiz</button>
<script>
const QUESTIONS = [
[" bonjour donner moi le nom du prof du php pour l'annee 2025 ?", "kamal el omari"],
[" Quelle est la capitale de  usa", "washintoon"], ["donner moi la somme de 22+3?", "25"],
["qulle est la voiture la plus celebre dans le maroc 
?", "Dacia"],
["67+33 ?", "100"]
];
function lancerQuiz() {
let bonnesReponses = 0;
for (let i = 0; i < QUESTIONS.length; i++) {
const question = QUESTIONS[i][0];
const reponseCorrecte = QUESTIONS[i][1].toLowerCase();
const reponseUtilisateur = prompt(question);
if (reponseUtilisateur !== null &&
reponseUtilisateur.trim().toLowerCase() ===
reponseCorrecte) {
alert("Réponse juste !");
bonnesReponses++;
} else {
alert("Réponse fausse !");
}
}
alert("Vous avez répondu correctement à " + bonnesReponses + "
question(s) sur " +
QUESTIONS.length + ".");
}
</script>
</body>
</html>
