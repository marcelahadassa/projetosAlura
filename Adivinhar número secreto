var numeroSecreto = Math.floor(Math.random() * 1000) + 1; //gera um número entre 1 e 100. Math.floor() arrendonda o número para garantir que temos um inteiro.
var nome = prompt("Qual o seu nome?");
var maxTentativas = 9;
var tentativas = 0;

while (tentativas < maxTentativas) {
  var valor = prompt(
    "Eai, " +
      nome +
      "! Digite um número entre 1 e 1000. Para desistir, insira 0"
  );
  if (valor == numeroSecreto) {
    alert("Você acertou!");
    break;
  } else if (valor > numeroSecreto) {
    alert(
      "Errou, o número é menor. Você tem " +
        (maxTentativas - tentativas - 1) +
        " chances."
    ); //conta feita para substrairmos as tentativas que são no max 6 e tentativas armazena o numero de tentativas que o jogador fez até agora (ela é incrementada a cada tentativa).
  } else if (valor == 0) {
    alert("Você desistiu! O número secreto era de " + numeroSecreto);
    break;
  } else {
    alert(
      "Errou, o número é maior. Você tem " +
        (maxTentativas - tentativas - 1) +
        " chances."
    );
  }
  tentativas++; //é incrementada apenas quando o jogador entra no bloco else if ou else (quando o jogador faz uma tentativa válida).
}

if (tentativas == maxTentativas) {
  alert("Suas chances acabaram. O número secreto era de " + numeroSecreto);
}
