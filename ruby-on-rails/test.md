#### Requirements
1. ActiveRecord & RSpec
- Tables
	- `users`: devise table
	  - extra fields: first_name(string, required), last_name(string), uuid(string, unique)
	- `subscriptions`
	- `user_subscriptions`
- Please add associations and validations in the each model
- Create 1 endpoint to create Stripe subscription
- Write RSpec test for the above endpoint
2. Sidekiq & RSpec
- Please add Sidekiq worker that imports CSV file into Database
- Please write RSpec test for the above worker
- Not required but a big plus: Please use Sidekiq `batch` feature
