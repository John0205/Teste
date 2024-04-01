//Questão 1
let INDICE = 13;
let SOMA = 0;
let K = 0;

while (K < INDICE) {
    K = K + 1;
    SOMA = SOMA + K;
}

console.log(SOMA);
//O valor da variável soma será 91.

//Questão 2

function isFibonacci(number) {
    let a = 0;
    let b = 1;
    let temp;

    while (a <= number) {
        if (a === number) {
            return true; 
        }
        temp = a;
        a = b;
        b = temp + b;
    }

    return false; 
}

const numeroInformado = 13;

if (isFibonacci(numeroInformado)) {
    console.log(numeroInformado + " pertence à sequência de Fibonacci.");
} else {
    console.log(numeroInformado + " não pertence à sequência de Fibonacci.");
}

//Questão 3

a)
let a = [1, 3, 5, 7];
let proximo_a = a[a.length - 1] + 2;

console.log("Próximo elemento da sequência a):", proximo_a);

b)
let b = [2, 4, 8, 16, 32, 64];
let proximo_b = b[b.length - 1] * 2;

console.log("Próximo elemento da sequência b):", proximo_b);
c)
let c = [0, 1, 4, 9, 16, 25, 36];
let proximo_c = c[c.length - 1] + (c.length * 2 + 1);

console.log("Próximo elemento da sequência c):", proximo_c);
d)
let d = [4, 16, 36, 64];
let proximo_d = Math.pow(d.length * 2, 2);

console.log("Próximo elemento da sequência d):", proximo_d);
e)
function fibonacci(n) {
    if (n <= 1)
        return n;
    else
        return fibonacci(n - 1) + fibonacci(n - 2);
}

let n = 7; 
let proximo_e = fibonacci(n);

console.log("Próximo elemento da sequência e):", proximo_e);
f)

let f = [2, 10, 12, 16, 17, 18, 19];
let proximo_f = f[f.length - 1] + 2;

console.log("Próximo elemento da sequência f):", proximo_f);

//Questão 4

//Primeiro, eu ligaria um dos interruptores e esperaria alguns minutos. Em seguida, desligaria esse interruptor e ligaria outro. Depois disso, entraria na sala onde as lâmpadas estão localizadas.
//Então, dependendo do que eu encontrasse lá dentro, poderia deduzir quais interruptores controlam quais lâmpadas. Se uma lâmpada estiver acesa, isso significa que o interruptor que eu liguei inicialmente controla essa lâmpada. Se estiver apagada e ainda estiver fria ao toque, isso indica que o interruptor que eu não toquei está controlando essa lâmpada. E se estiver apagada, mas ainda estiver quente ao toque, isso sugere que o interruptor que eu liguei inicialmente controla essa lâmpada.

//Questão 5

function inverterString(str) {
    let novaString = '';
    for (let i = str.length - 1; i >= 0; i--) {
        novaString += str[i];
    }
    return novaString;
}


const minhaString = "Olá, mundo!";
const stringInvertida = inverterString(minhaString);
console.log("String original:", minhaString);
console.log("String invertida:", stringInvertida);
