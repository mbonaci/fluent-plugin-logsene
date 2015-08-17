# Fluent::Plugin::Logsene, a plugin for [Fluentd](http://fluentd.org)

fluent output plugin for [Logsene](http://sematext.com/logsene)

## Fluentd
http://fluentd.org/

## Logsene
http://www.sematext.com/logsene

## Installation

Add this line to your application's Gemfile:

    gem 'fluent-plugin-logsene'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install fluent-plugin-logsene

## Usage
Simply replace the dummy application token in the `path` configuration setting with the one you can find on the `App Actions > App Settings` or the `Integration` page when you sign in on [sematext.com](sematext.com).

      <match *.apache.*>
        type logsene
        host logsene-receiver.sematext.com
        port 80
        format json|text
        path /5233x41x-3xx5-8754-x354-xxx1x018ex33x
      </match>


#### type
- logsene

#### host
- Hostname of HTTP Collectors URL

#### port
- Port of HTTP Collectors URL

#### path
- Path of HTTP Collectors URL

#### format
- json: send as json

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
