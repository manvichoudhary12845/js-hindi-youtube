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
#project 2
``` javascript
const form = document.querySelector('form');
form.addEventListener('submit',function(e){
  e.preventDefault();

  const height = parseInt(document.querySelector('#height').value);
  const weight = parseInt(document.querySelector('#weight').value);
  const results = document.querySelector('#results');

  if (height ===""|| height<0 ||isNaN(height)){
    results.innerHTML=`please give a valid height ${height}`;
  }
  else if (weight === ""|| weight<0 ||isNaN(weight)){
    results.innerHTML=`please give a valid weight ${weight}`;
  }
  else {
    
    const bmi = (weight / ((height / 100) * (height / 100))).toFixed(2);
  if(bmi<=18.6) {
      results.innerHTML =`<span>Under Weight:${bmi}</span>`;
  }
  else if(bmi>18.6 && bmi<=24.6){
    results.innerHTML =`<span>normal range:${bmi}</span>`;
  }
  else if (bmi>24.6){
    results.innerHTML =`<span> Over weight: ${bmi}</span>`;
  }
  }
    //show the result
    //results.innerHTML =`<span>${bmi}</span>`;
    
  
});
```
