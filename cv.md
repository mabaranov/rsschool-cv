# Resume
1. Mikhail Baranov
1. Contact info: mail.baranov@gmail.com
1. Goals: I want to go to web programming
1. Skills: C/C++, 1C, HTML and CSS basics, JS basics, git.
1. Code example:
```javascript
import readlineSync from 'readline-sync';

const countAttempt = 3;

const play = (game, rule) => {
  console.log('Welcome to the Brain Games!');
  console.log(`${rule}\n`);

  const name = readlineSync.question('May I have your name? ');
  console.log(`Hello, ${name}`);

  for (let i = 0; i < countAttempt; i += 1) {
    const gameStep = game();
    console.log(`Question: ${gameStep.question}`);
    const userAnswer = readlineSync.question('Your answer: ');

    if (gameStep.answer === userAnswer) {
      console.log('Correct!');
    } else {
      console.log(`'${userAnswer}' is wrong answer ;(. Correct answer was '${gameStep.answer}'.\nLet's try again, '${name}'!\n`);
      return;
    }
  }
  console.log(`Congratulations, ${name}! \n`);
};

export { play as default };
```
6. Works.
1. Education: HTML and CSS, level 1 (htmlacademy.).
1. English: A1 level.
