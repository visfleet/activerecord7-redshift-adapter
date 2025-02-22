activerecord7-redshift-adapter
==============================

Amazon Redshift adapter for ActiveRecord 7 (Rails 7).
This is a fork from https://rubygems.org/gems/activerecord7-redshift-adapter hosted on a private Gitlab instance.
It's itself forked the project from https://github.com/kwent/activerecord6-redshift-adapter

Thanks to the auhors.

Usage
-------------------

For Rails 7, write following in Gemfile:

```ruby
gem 'activerecord7-redshift-adapter', git: 'https://github.com/pennylane-hq/activerecord7-redshift-adapter.git'
```

In database.yml

```YAML
development:
  adapter: redshift
  host: host
  port: port
  database: db
  username: user
  password: password
  encoding: utf8
```

OR your can use in URL
```ruby
class SomeModel < ApplicationRecord
  establish_connection('redshift://username:password@host/database')
end
```

License
---------

MIT license (same as ActiveRecord)
