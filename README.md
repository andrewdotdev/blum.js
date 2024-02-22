# @blumqa/astrology

## What is it?

It's' a package to use dynamic q&a (questions and answers) of astrology

## How to install

```bash
pnpm install @blumqa/astrology
```

I will use pnpm but you can use any other like npm.

## How to use

There are 2 functions
```ts
/**
 * 
 * @param lang Options are 'en' and 'es'
 * @param id The id of the q&a
*/
getRandom(lang: string)
getById(lang: string, id: number)
```
## Example
```ts
const { getRandom, getById } = require('@blumqa/astrology')

console.log(getRandom('en')) // Output: {id: number, question: string, answer: string, options: string[]}
console.log(getById('es', 5)) // Output: {id: 5, question: "¿Quién fue el primer cosmonauta en viajar al espacio?", answer: "Yuri Gagarin", options: ["Neil Armstrong", "Buzz Aldrin", "Yuri Gagarin", "Alan Shepard"]}
```