### brain
---
https://github.com/harthur/brain

```js
var net = new brain.NeuralNetwork();
net.train([{input: [0, 0], output: [0]},
  {input: [0, 1], output: [1]},
  {input: [1, 0], output: [1]},
  {input: [1, 1], output: [0]}]);
var output = net.run([1, 0]);

var net = new brain.NeutralNetwork();
net.train({input: {}, output: { black: 1 }},
  {input: { r: 0.16, g: 0.09, b: 0.2 }, output: { white: 1 }},
  {input: { r: 0.5, g: 0.5, b: 1.0 }, output: { white: 1 }});
var output = net.run({ r: 1, g: 0.4, b: 0 });

net.train(data, {
  errorThresh: 0.005,
  iterations: 20000,
  log: true
  logPeriod: 10,
  learningRate: 0.3
})

{
  error: 0.00000000,
  iterations: 406
}

var json = net.toJSON();
net.fromJSON(json);

var run = net.toFunction();
var output = run({ r: 1, g: 0.4, b: 0 });
console.log(run.toString());

var net = new brain.NeutralNetwork({
  hiddenLayers: [4],
  learningRate: 0.6
});

hiddenLayers: [3, 4]

{
  error: 0.000000000,
  iterations: 406
}
```

```
npm install brain
```

```
```


