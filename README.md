# AzulPayButton

This is a simple gem to integrate Azul Payment Page in your Ruby on Rails app.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'azul_pay_button'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install azul_pay_button

## Usage

run in the terminal:

    $ rails g azul

Edit the config file in /config/azul_config.yml

and use this snippet in your view:

```ruby
<%= azul_pay_button(order_number, currency, amount, itbis) %>
```
Where:

* order_number: is the order number of your transation.

* currency: must be "$" to indicate DOP or "US$" to indicate Dollars. Others currency not work.

* amount: is the price of your products, this value is add up to the itbis

* itbis: this value not must be in percentage, must be in decimals or number.

And enjoy it!! 😎

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/azul_pay_button. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
