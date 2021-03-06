# Mohair

## Installation

Add this line to your application's Gemfile:

    gem 'mohair'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install mohair

## Usage

now:

```
$ bundle exec bin/mohair -q "select all from sometable" -i INDEX
$ bundle exec bin/mohair_dump < data.json
```

future:

```
$ bundle exec bin/mohair -i
mohair> select * from sometable
mohair> insert * into ...
mohair>
```

```
$ bundle exec bin/mohair -q "select * from sometable"
...
```

## Currently works

- basic SQL parsing
- select * from table
- select col,col,col from table [where col = "name" and col < 23] [group by col]

## TODO

- limit 10
- asc/desc
- types: timestamp, float
- recursive representation of json with dot notation
- 2i
- query optimization

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

```
$ rake release
```
