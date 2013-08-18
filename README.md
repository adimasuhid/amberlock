# Amberlock

Two-factor Authentication via SMS/Email. Ruby gem API for https://rubygems.org/gems/amberlock

## Installation

Add this line to your application's Gemfile:

    gem 'amberlock'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install amberlock

## Usage

Log-in to AmberLock (http://amberlock.herokuapp.com) and create a new amber app.

Instantiate your amber app

    amber = Amberlock::Amber.new('[YOUR API KEY]','[APP AMBER CODE]')

To register a user to your amber app

    amber.subscribe_user('[mobile number]','[email number]')

To request for an amber authentication key for your user

    amber.request_unlock('[mobile number]','[email number]')

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
