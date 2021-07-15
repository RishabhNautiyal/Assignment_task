const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.on('line', (input) => {
  
for(i=1;i<=input;i++){
  let x="";
  if(i%2===0){
    for(j=i;j>=1;j--){
      x= `${x} ${j}`;
    }
    console.log(`${x}\n`);
  } else {
    for(j=1;j<=i;j++){
      x= `${x} ${j}`;
    }
    console.log(`${x}\n`);
  }
}

for(i=input-1;i>=1;i--){
  let x="";
  if(i%2===0){
    for(j=i;j>=1;j--){
      x= `${x} ${j}`;
    }
    console.log(`${x}\n`);
  } else {
    for(j=1;j<=i;j++){
      x= `${x} ${j}`;
    }
    console.log(`${x}\n`);
  }
}

});

