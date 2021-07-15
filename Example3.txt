const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.on('line', (input) => {
  
  number = 1;
  
  if(input%2 === 0 ) {
    for(var i = 1; i<=input-1; i++) {
      console.log(number);
      number +=2;
    }
  } else {
    for(var i = 1; i<=input; i++) {
      console.log(number);
      number +=2;
    }
  }  
});
