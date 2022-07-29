activerecord7-redshift-adapter
==============================

Built on https://github.com/persado/activerecord6-redshift-adapter

Usage
-------------------

For Rails 7, write following in Gemfile:

```ruby
gem 'activerecord7-redshift-adapter'
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
