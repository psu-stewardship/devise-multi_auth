# Devise::MultiAuth [![Build Status](https://travis-ci.org/jeremyf/devise-multi_auth.png?branch=master)](https://travis-ci.org/jeremyf/devise-multi_auth) [![Version](https://badge.fury.io/rb/devise-multi_auth.png)](http://badge.fury.io/rb/devise-multi_auth)

A [Devise](https://github.com/plataformatec/devise) plugin leveraging [omniauth](https://github.com/intridea/omniauth) to
expose alternate means for authenticating existing users.

```gherkin
Scenario: As a Developer
Given that I am using Devise
And that I have an existing user Signup process
When I use Devise::MultiAuth
Then I can expose alternate means of authenticating existing users.
```

## Getting Started

Add the following line to your application's Gemfile:

    gem 'devise-multi_auth'

And then execute:
```bash
$ bundle
$ rails generate devise:multi_auth:install
```

## TODO

At present, this [Rails Engine](http://guides.rubyonrails.org/engines.html) does not expose an obvious means for initiating the connecting between an existing account and an omniauth-enabled account (i.e. login via Github).