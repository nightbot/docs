/*
Title: Eval
*/

The Eval variable is used to evaluate JavaScript code. The timeout length of the script execution is 1 second. 

## Usage

> $(eval `javascript`)

#### Example Usage

> $(eval 2 + 2)

would result in 

> 4

### Example Usage

> $(eval for(;;){}) `(infinite loop)`

would results in

> Script execution timed out.

## Examples

#### Generate a random number between 1 to 100

> !commands add !random The Random Number is: $(eval Math.floor((Math.random() * 100) + 1))

#### Make an 8ball command

> !commands add !8ball 🎱 $(eval const responses = ['All signs point to yes...', 'Yes!', 'My sources say nope.', 'You may rely on it.', 'Concentrate and ask again...', 'Outlook not so good...', 'It is decidedly so!', 'Better not tell you.', 'Very doubtful.', 'Yes - Definitely!', 'It is certain!', 'Most likely.', 'Ask again later.', 'No!', 'Outlook good.', 'Don\\'t count on it.']; responses[Math.floor(Math.random() * responses.length)];)
