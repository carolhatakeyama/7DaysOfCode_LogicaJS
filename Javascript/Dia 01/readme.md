# Dia 01 - Trabalhando com operadores lógicos em Javascript

### Tópicos
- [Tecnologias Usadas](#tecnologias-usadas)
- [Desafio](#desafio)
  - [Dica](#dica)
  - [Extra](#extra)
- [Resposta](#resposta)
  - [Resposta Alura](#resposta-alura)

## Tecnologias Usadas

*   Javascript

## Desafio

Este primeiro dia é super importante! Ao final dele, você terá um novo conhecimento que é essencial para os próximos desafios.

Existe uma situação super comum para quem utiliza o Javascript: problemas com os tipos de variáveis na hora de comparar os valores de duas variáveis entre si. Eu já passei muito por isso!

Em linguagens de programação compiladas, como Java e C#, esse problema é detectado em tempo de compilação, e você que está desenvolvendo o código tem um aviso claro do erro.
Já no Javascript, esses erros passam despercebidos, já que o código não passa por um compilador. Ou seja, os erros só aparecem em tempo de execução. 

A parte mais confusa para quem está começando a aprender lógica com Javascript é a operação de igualdade entre valores. Dependendo de como você escrever o seu código, o Javascript fará uma conversão de tipo para um tipo booleano de maneira implícita (automática), e isso afetará variáveis que eram Strings, Numbers, Object, etc….

Isso causa alguns comportamentos estranhos, como todos esses exemplos aqui abaixo retornando true:

```
  console.log( false == '0' );
  console.log( null == undefined );
  console.log( " \t\r\n" == 0 );
  console.log( ' ' == 0 );
```  

O que não faz necessariamente muito sentido.

(Você pode testar tudo isso indo no seu navegador, clicando com o botão direito, escolhendo a opção "Inspecionar" e a aba "Console". Nessa aba, basta copiar e colar cada uma das linhas acima para confirmar que todas realmente retornam true).


Sendo assim, a sua tarefa de hoje é reescrever o código abaixo de maneira que ele imprima as informações de maneira correta, que faça sentido e sem erros:

```
  let numeroUm = 1
  let stringUm = '1'
  let numeroTrinta = 30
  let stringTrinta = '30'
  let numeroDez = 10
  let stringDez = '10'


  if (COMPARAR O numeroUm e a stringUm) {
    console.log('As variáveis numeroUm e stringUm tem o mesmo valor, mas tipos diferentes')
  } else {
    console.log('As variáveis numeroUm e stringUm não tem o mesmo valor')
  }

if (COMPARAR O numeroTrinta e a stringTrinta) {
  console.log('As variáveis numeroTrinta e stringTrinta tem o mesmo valor e mesmo tipo')
} else {
  console.log('As variáveis numeroTrinta e stringTrinta não tem o mesmo tipo')
}

if (COMPARAR O numeroDez e a stringDez) {
  console.log('As variáveis numeroDez e stringDez tem o mesmo valor, mas tipos diferentes')
} else {
  console.log('As variáveis numeroDez e stringDez não tem o mesmo valor')
}

```

### Dica
Você também pode utilizar o próprio navegador para executar esse seu programa, caso ainda não tenha familiaridade com editores de código, como o Visual Studio Code.

Para isso, como eu falei acima, basta você clicar com o botão direito do mouse em qualquer página, selecionar a opção "Inspecionar", ir na aba "Console" e digitar o seu código. Bem simples, né?

Se você quiser mudar os nomes das variáveis e valores, fique à vontade. Mas jamais imprima algo que não seja verdadeiro, hein!

### Extra
#### Como utilizar operadores de comparação em Javascript
Para cada tipo de comparação, temos um operador diferente:

| Operador | Operação | Exemplo 
| -------- | -------- | -------                
| >   | Maior que        | (a > b)
| <	  | Menor que	     | (a < b)
| >=  | Maior ou igual a | (a >= b)
| <=  | Menor ou igual a | (a <= b)
| ==  | Igual a          | (a == b)
| !=  | Diferente de	 | (a !== b)
| === | Idêntico a       | (a === b)
| !== |	Não idêntico a   |	(a !== b)
| &&  |	E/and            |	(a && b)
| ll  |	Ou/or            |	(a ll b)

#### Diferença entre “==” e “===”
O símbolo de “igual a” (==) realiza a validação apenas do caractere.

O símbolo de “idêntico a” (===) compara não apenas os valores mas também verifica se são do mesmo tipo.

E assim como os operadores “==” e “===”, usamos a mesma lógica para os seus inversos “!=” e “!==”.

#### Referências 
* [Artigo Alura](https://www.alura.com.br/artigos/operadores-matematicos-em-javascript?gclid=Cj0KCQiA_8OPBhDtARIsAKQu0gYUqZqgonpXyEP1_hpUl58wYAk_P3Ze4VWrxo9ftkFW9CLYOMyjO1caAlrzEALw_wcB&utm_source=ActiveCampaign&utm_medium=email&utm_content=%237DaysOfCode+-+L%C3%B3gica+JS+1%2F7%3A+Opera%C3%A7%C3%B5es+Booleanas&utm_campaign=%5BALURA+%237days+Of+Code%5D+%28L%C3%B3gica+de+Programa%C3%A7%C3%A3o+-+JavaScript%29+Dia+1%3A+Comparando+Valores&vgo_ee=F9c%2FFeXJKtFaSDiEzuuGvL35hO7C%2FF3J%2FgQB9Uu3XAY%3D)

## Resposta
```
let numeroUm = 1
let stringUm = '1'
let numeroTrinta = 30
let stringTrinta = '30'
let numeroDez = 10
let stringDez = '10'

if (numeroUm == stringUm & numeroUm !== stringUm) {
  console.log('As variáveis numeroUm e stringUm tem o mesmo valor, mas tipos diferentes')
} else if (numeroUm != stringUm) {
  console.log('As variáveis numeroUm e stringUm não tem o mesmo valor')
}

if (numeroTrinta === stringTrinta) {
console.log('As variáveis numeroTrinta e stringTrinta tem o mesmo valor e mesmo tipo')
} else {
 console.log('As variáveis numeroTrinta e stringTrinta não tem o mesmo tipo')
}

if (numeroDez == stringDez & numeroDez !== stringDez) {
 console.log('As variáveis numeroDez e stringDez tem o mesmo valor, mas tipos diferentes')
} else if (numeroDez != stringDez) {
  console.log('As variáveis numeroDez e stringDez não tem o mesmo valor')
}
```

### Resposta Alura
```
let numeroUm = 1
let stringUm = '1'
let numeroTrinta = 30
let stringTrinta = '30'
let numeroDez = 10
let stringDez = '10'

if (numeroUm == stringUm) {
  console.log('As variáveis numeroUm e stringUm tem o mesmo valor, mas tipos diferentes')
} else {
  console.log('As variáveis numeroUm e stringUm não tem o mesmo valor')
}

if (numeroTrinta === stringTrinta) {
  console.log('As variáveis numeroTrinta e stringTrinta tem o mesmo valor e mesmo tipo')
} else {
  console.log('As variáveis numeroTrinta e stringTrinta não tem o mesmo tipo')
}

if (numeroDez == stringDez) {
  console.log('As variáveis numeroDez e stringDez tem o mesmo valor, mas tipos diferentes')
} else {
  console.log('As variáveis numeroDez e stringDez não tem o mesmo valor')
}
```
