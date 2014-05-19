* Match arrays in different order `array.should =~ another_array`
* Expect a change of value
```
  expect{ Counter.increment }.to change{ Counter.count }.by(2)
  expect{ Counter.increment }.to change{ Counter.count }.from(0).to(2)
```
* [Using Devise in controller specs](https://github.com/plataformatec/devise/wiki/How-To%3a-Controllers-tests-with-Rails-3-%28and-rspec%29)
* When using `user_signed_in?` or other Devise stuff in controller / view specs:
```
RSpec.configure do |config|
  config.include Devise::TestHelpers, :type => :controller
  config.include Devise::TestHelpers, :type => :view
end
```
* Stub will_paginate `view.stub(:will_paginate)`
* [How to test mailers with rspec](http://blog.lucascaton.com.br/index.php/2010/10/25/how-to-test-mailers-in-rails-3-with-rspec/)
