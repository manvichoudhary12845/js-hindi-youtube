# Projects related to DOM

## Project link
[Click here] (https://stackblitz.com/edit/dom-project-chaiaurcode?file=index.html)

# Solution code 

## Project 1 
```javascript
console.log("hitesh")

const buttons = document.querySelectorAll('.button');
const body = document.querySelector("body");

buttons.forEach(function (button){
button.addEventListener('click',function(e){
    console.log(e);
    console.log(e.target)
    if(e.target.id==='grey'){
      body.style.background =e.target.id;
    }
    if(e.target.id==='white'){
      body.style.background =e.target.id;
    }
    if(e.target.id==='blue'){
      body.style.background =e.target.id;
    }
    if(e.target.id==='yellow'){
      body.style.background = e.target.id;
    }
});
});

```
