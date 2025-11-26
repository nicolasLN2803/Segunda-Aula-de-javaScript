📘 INFINITY SCHOOL

🎨 VISUAL ART CREATIVE CENTER

JavaScript – Aula 02
Operadores Lógicos • Comparação • Condicionais • Ternário • Switch
📚 O QUE IREMOS APRENDER
Nº	Conteúdo
01	Revisão da Aula Anterior
02	Operadores Lógicos
03	Operadores de Comparação
04	Condicionais (if / else if / else)
05	Ternário
06	Switch
🔄 01 – Revisão da Aula Anterior
Conteúdos revisados:

Introdução ao JavaScript

alert() e console.log()

Variáveis (var, let, const)

Tipos de Dados

Entrada de Dados (prompt, confirm)

Operadores Aritméticos

Operadores de Atribuição

Concatenação e Template Strings

🔐 02 – OPERADORES LÓGICOS

Os operadores lógicos combinam expressões booleanas e retornam true ou false.

Os três principais:
Operador	Significado	Descrição
&&	AND (E)	Retorna true se ambos forem verdadeiros
`		`
!	NOT (NÃO)	Inverte o valor booleano
🟩 Operador AND (&&)

Retorna true somente se ambos forem verdadeiros.

A	B	A && B
true	true	true
true	false	false
false	true	false
false	false	false
🟧 Operador OR (||)

Retorna true se pelo menos um for verdadeiro.

A	B	A || B
true	true	true
true	false	true
false	true	true
false	false	false
🟥 Operador NOT (!)

Inverte o valor.

A	!A
true	false
false	true
📝 Atividade Prática 01 – Operadores Lógicos

Solicite dois números ao usuário e verifique:

Se ambos são positivos → &&

Se pelo menos um é positivo → ||

Se nenhum é positivo → !

let numero1 = Number(prompt("Digite o primeiro número:"));
let numero2 = Number(prompt("Digite o segundo número:"));

console.log("Ambos positivos?", numero1 > 0 && numero2 > 0);
console.log("Pelo menos um positivo?", numero1 > 0 || numero2 > 0);
console.log("Nenhum positivo?", !(numero1 > 0) && !(numero2 > 0));

⚖️ 03 – OPERADORES DE COMPARAÇÃO

Comparam valores e retornam true ou false.

Operador	Nome	Descrição
==	Igualdade	Compara valor com conversão automática
===	Igualdade Estrita	Compara valor e tipo
!=	Diferente	Compara valores
!==	Diferente Estrito	Compara valor e tipo
>	Maior que	—
>=	Maior ou igual	—
<	Menor que	—
<=	Menor ou igual	—
🔍 Igualdade vs Igualdade Estrita
5 == "5"   // true
5 === "5"  // false

📝 Atividade Prática 02 – Comparação

Solicite dois números e compare-os usando todos os operadores.

let numero1 = Number(prompt("Digite o primeiro número:"));
let numero2 = Number(prompt("Digite o segundo número:"));

console.log("==", numero1 == numero2);
console.log("===", numero1 === numero2);
console.log("!=", numero1 != numero2);
console.log("!==", numero1 !== numero2);
console.log(">", numero1 > numero2);
console.log("<", numero1 < numero2);
console.log(">=", numero1 >= numero2);
console.log("<=", numero1 <= numero2);

🧠 04 – CONDICIONAIS

Permitem executar blocos diferentes de código dependendo da condição.

Estruturas:

if

else if

else

switch

🟦 IF (SE)
if (condicao) {
  // código se a condição for verdadeira
}

🟨 ELSE IF (SENÃO SE)
if (cond1) {
} else if (cond2) {
}

🟥 ELSE (SENÃO)
if (cond1) {
} else {
}

📝 Atividade Prática 03 – Positivo, Negativo ou Zero
let numero = Number(prompt("Digite um número:"));

if (numero > 0) {
  console.log("Número positivo");
} else if (numero < 0) {
  console.log("Número negativo");
} else {
  console.log("Zero");
}

✨ 05 – Ternário

Forma curta de um if/else.

condicao ? valorSeVerdadeiro : valorSeFalso;

Exemplo
let idade = 20;
let status = idade >= 18 ? "maior de idade" : "menor de idade";

🔄 Comparação com if-else
let status;

if (idade >= 18) {
  status = "maior de idade";
} else {
  status = "menor de idade";
}

🔀 06 – SWITCH

Usado quando queremos verificar múltiplos valores.

switch (expressao) {
  case valor1:
    // código
    break;

  case valor2:
    // código
    break;

  default:
    // se nenhum caso for correspondido
}

📝 Atividade Prática 04 – Calculadora com Switch
let numero1 = Number(prompt("Digite o primeiro número:"));
let numero2 = Number(prompt("Digite o segundo número:"));
let operacao = prompt("Digite a operação (+, -, *, /):");

switch (operacao) {
  case "+":
    console.log(numero1 + numero2);
    break;

  case "-":
    console.log(numero1 - numero2);
    break;

  case "*":
    console.log(numero1 * numero2);
    break;

  case "/":
    console.log(numero1 / numero2);
    break;

  default:
    console.log("Operação inválida!");
}
