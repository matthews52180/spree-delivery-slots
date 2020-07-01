SpreeDeliverySlots
==================

SpreeDeliverySlots allows customer to select preferred delivery time for his order. Admin can add a number of time slots(ex: 11:00 AM - 3 PM and 4 PM - 9PM) when he can deliver from shipping method edit/new page. Customer will be able to select only from these pre-created time slots.

Demo
-----------------------------------
Try Spree Delivery Slots for Spree Master with direct deployment on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/vinsol-spree-contrib/spree-demo-heroku/tree/spree-delivery-slots-master)

Try Spree Delivery Slots for Spree 4-1 with direct deployment on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/vinsol-spree-contrib/spree-demo-heroku/tree/spree-delivery-slots-4-1)

Try Spree Delivery Slots for Spree 3-4 with direct deployment on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/vinsol-spree-contrib/spree-demo-heroku/tree/spree-delivery-slots)

Try Spree Delivery Slots for Spree 3-1 with direct deployment on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/vinsol-spree-contrib/spree-demo-heroku/tree/spree-delivery-slots-3-1)

Features
--------

* While placing the order customer will be able to select the delivery time while selecting the shipping method.

* Once a order has been placed admin will be able to see the preffered delivery time in order's shipment page and can deliver accordingly.

* Delivery slot info will also be present in shipped email.

Installation
------------

1. Add this extension to your Gemfile with this line:

  #### Spree > 3.3

  ```ruby
    gem 'spree_delivery_slots', git: 'https://github.com/vinsol-spree-contrib/spree-delivery-slots', branch: 'master'
  ```

  #### Spree <= 3.3

  ```ruby
    gem 'spree_delivery_slots', git: 'https://github.com/vinsol-spree-contrib/spree-delivery-slots', branch: 'X-X-stable'
  ```

  The `branch` option is important: it must match the version of Spree you're using.
  For example, use `3-0-stable` if you're using Spree `3-0-stable` or any `3.0.x` version.


2. Install the gem using Bundler:
  ```ruby
    bundle install
  ```

3. Copy & run migrations
  ```ruby
    bundle exec rails g spree_delivery_slots:install
  ```

4. Restart your server

  If your server was running, restart it so that it can find the assets properly.


Testing
-------

  #### Spree >= 3.1

  For Building Dependencies:
  ```shell
  appraisal install
  ```

  The dummy app can be regenerated by using:
  ```shell
  appraisal spree-3-1 rake test_app

  ```
  This will run rake test_app using the dependencies configured for Spree 3.1. Similarly you can use spree-3-2 and spree-master for generating dummy applications using dependencies for Spree 3.2 and latest version of Spree


  ```shell
  appraisal spree-3-1 rspec
  ```
  This will run rspec using the dependencies configured for Spree 3.1. Similarly you can use spree-3-2 and spree-master to run rspec using dependencies for Spree 3.2 and latest version of Spree


  #### Spree 3.0 and Spree 2.x

  First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

  ```shell
  bundle
  bundle exec rspec spec
  ```

  ## See It In Action
  
  <a href="http://www.youtube.com/watch?feature=player_embedded&v=iqbrRheTQNw
" target="_blank"><img src="http://img.youtube.com/vi/iqbrRheTQNw/0.jpg" 
alt="Youtube Video Tutorial" /></a>

Contributing
------------

  1. Fork the repository.
  2. Clone your repository.
  3. Run `bundle install`.
  5. Make the required changes.
  6. Ensure all specs are passing.
  7. Submit your pull request.

Credits
-------

[![vinsol.com: Ruby on Rails, iOS and Android developers](http://vinsol.com/vin_logo.png "Ruby on Rails, iOS and Android developers")](http://vinsol.com)

Copyright (c) 2017 [vinsol.com](http://vinsol.com "Ruby on Rails, iOS and Android developers"), released under the New MIT License
