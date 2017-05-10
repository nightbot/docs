/*
Title: Eval
*/

The Eval variable is used to evaluate JavaScript code. The timeout length of the script execution is 2 seconds. 

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

!commands add !random The Random Number is: $(eval Math.floor((Math.random() * 100) + 1))