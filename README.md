# Deadlock Retry INSANE EDITION (more retries)

Deadlock retry allows the database adapter (currently only tested with the
MySQLAdapter) to retry transactions that fall into deadlock. It will retry
such transactions three times before finally failing.

This capability is automatically added to ActiveRecord. No code changes or otherwise are required.

## Installation

Add it to your Rails application by installing the gem:

  gem install deadlock_retry_insane

and including a reference to it in your application's Gemfile:

  gem 'deadlock_retry_insane', require: 'deadlock_retry'

## Original Authors

Jamis Buck and Mike Perham made it. I just changed a number.
