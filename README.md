# Jungle

A mini e-commerce application built with Rails 6.1 for purposes of learning Rails by example. An online store selling flowers, bushes, trees, and anything else. Stripe payments and user authentication are featured.

## Demo

Checking out with sign in:
!["Jungle Home Screen and Anonymous Checkout Flow"](https://github.com/Wilson-Chu/jungle/blob/master/docs/home_journey.gif?raw=true)

Signing up new user and navigating Admin Dashboard:
!["Admin Dashboard Demo and Logged-in Checkout Flow"](https://github.com/Wilson-Chu/jungle/blob/master/docs/signup_auth_checkout_journey_1080p.gif?raw=true)

## Setup

1. If using SSH:
```
git clone git@github.com:Wilson-Chu/jungle.git
```
2. From home directory:
```
cd jungle
```
3. Run `bundle install` to install dependencies
4. Run `bin/rails db:reset` to create, load and seed db 

- You may have to start up your PostgreSQL system, from the terminal:
```
$ startpostgres
=> Enter password (if applicable)

$ psql jungle_development
=> Enter password (if applicable)
```

5. Run `bin/rails s -b 0.0.0.0` to start the server

The website will be hosted on http://localhost:3000 by default.


## Stripe Testing

Use Credit Card # 4111 1111 1111 1111 for testing success scenarios. 

Expiry date can be the current month or anytime in the future. CVV can be anything for testing.

More information in their docs: <https://stripe.com/docs/testing#cards>

## Dependencies

- Rails 6.1 [Rails Guide](http://guides.rubyonrails.org/v6.1/)
- Bootstrap 5
- PostgreSQL 9.x
- Stripe
