# Install Jest using npm
`npm install --save-dev jest`


## Let's get started by writing a test for a hypothetical function that adds two numbers. First, create a sum.js file:
`function sum(a, b) {
  return a + b;
}
module.exports = sum;`


## Then, create a file named sum.test.js. This will contain our actual test:
`const sum = require('./sum');

test('adds 1 + 2 to equal 3', () => {
  expect(sum(1, 2)).toBe(3);
});`


## Add the following section to your package.json:
`{
  "scripts": {
    "test": "jest"
  }
}`


## Finally, run npm test and Jest will print this message:
`PASS  ./sum.test.js
✓ adds 1 + 2 to equal 3 (5ms)`

## You just successfully wrote your first test using Jest!

This test used expect and toBe to test that two values were exactly identical. [Source:] (https://jestjs.io/docs/getting-started)