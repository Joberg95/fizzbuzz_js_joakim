# FIZZBUZZ IN JS [WIP]

## Question 1: Explain this code snippet and what it does.
```javascript
let  fizzBuzz = fs.readFileSync('./src/js/fizz-buzz.js');
eval( fizzBuzz + `\nexports.FizzBuzz = FizzBuzz;`)
```
Answer: Returns content in a callback.

## Question 2. To the best of your knowledge please explain why we are placing the let fizzBuzz = new FizzBuzz outside the it block?

Answer: -

## Question 3. To the best of your knowledge please explain the difference between using === and == in JS?

Answer: '==' compares only value, while '===' checks value as well as type.

## Question 4. To the best of your knowledge please explain why we are moving (number % 5 === 0) to the top?

Answer: It needs to be on top since the function runs from top to bottom.

## Question 5. To the best of your knowledge please explain the difference between feature and unit test

Answer: Unit testing tests specific functions while feature testing is testing the things our user sees.

## Question 6. To the best of your knowledge please explain what this following code does

```javascript
describe('User can input a value and get FizzBuzz results', () => {
    before(async () => {
        await  browser.init()
        await  browser.visitPage('http://localhost:8080/')
    });

    beforeEach(async () => {
        await  browser.page.reload();
    })

    after(async ()=> {
        await  browser.close();
    })
})
```
Answer: It sets up a test browser using a default browser port called 8080 and closes it after the tests are done.

## Question 7. To the best of your knowledge please explain what expectations in the context of testing are

Answer: (not sure how to answer this) But we write tests in a certain way to fix specific issues in our code.

## to the best of your knowledge please write a line to line explanation of what is happening in this code

```javascript
<script src="./js/fizz-buzz.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            let button = document.getElementById('button')
            let displayDiv = document.getElementById('display_answer')
            button.addEventListener('click', () =>{
                let value = document.getElementById('value').value
                let fizzBuzz = new FizzBuzz
                let result = fizzBuzz.check(value)
                displayDiv.innerHTML = result;
            })
        })
    </script>
```
Answer: ```<script src="">``` is the link to our actual js fizzbuzz code. And the rest is linked to the "eventlistener" which loads the content once the page is open.

## Question 9. To the best of your knowledge please explain what a CDN (Content Delivery Network) is?

Answer: (in short) A content delivery network (CDN) is a system of distributed servers that deliver pages and other Web content to a user.


