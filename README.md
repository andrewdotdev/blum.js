# Blum.js
## What is it?
It's' a package to use dynamic q&a (questions and answers)
## How to install
```bash
pnpm install blum.js
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
const { getRandom, getById } = require('blum.js')

console.log(getRandom('en'))
console.log(getById('es', 5))
```