This file is a simple Ruby RSpec test suite describing a DeliveryRouter class.
Your goals are to:
1) make those tests pass,
2) add tests for the edge cases.

To setup the project, perform the following actions from a Ruby 2.x environment:
---
```
gem install bundler
cat >Gemfile <<END
source "https://rubygems.org"
gem 'rspec', '~> 3.0'
END
bundle install
rspec --init
```
---

Then put the "delivery_router_spec.rb" test suite file in the spec/ folder,
and create a lib/delivery_router.rb file which should hold the DeliveryRouter class.

Your project tree should look like this:
.
```
├── Gemfile
├── Gemfile.lock
├── lib
│   └── delivery_router.rb
└── spec
  ├── delivery_router_spec.rb
  └── spec_helper.rb
```
To run the tests, just type "rspec" on the command line.
Feel free to ask us any question!

Happy hacking :)

--

Goal: delight your customers by sending riders to pick and deliver their orders
in less than 60 minutes (faster if you can).

Hypothesis:
- (x, y) coordinates are used to locate restaurants, customers and riders on a grid
- the distance between x=0 and x=1 is 1000 meters (1 km)
- the distance between two arbitrary (x,y) locations is the euclidian distance (straight line)
- times are expressed in minutes
- speeds are expressed in kilometers per hour (km/h)

Note: some other hypothesis you can make to simplify the problem:
- all customer orders are received at the same time (t=0)
- all restaurants start cooking at the same time (t=0)
- all riders start moving at the same time (t=0)
- each restaurant can cook an infinite number of meals in parallel
- each rider can carry an infinite amount of meals at the same time
- riders are ninjas! They fly over trafic jams and buildings, they never need to take
  a break and they know how to solve a NP-complete problem in polynomial time ;)
