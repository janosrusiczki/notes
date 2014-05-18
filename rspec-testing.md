* Match arrays in different orders `array.should =~ another_array`
* Expect a change of value
```
  expect{ Counter.increment }.to change{ Counter.count }.by(2)
  expect{ Counter.increment }.to change{ Counter.count }.from(0).to(2)
```
