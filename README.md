# Devise Bootstrap Views

Here are some of the highlights:

- Devise views with Bootstrap 5
- Responsive layout
- I18n support

![Screenshot](https://raw.githubusercontent.com/asecondwill/devise-bootstrap-views/master/Screenshot.png)

## Installation

Make sure Bootstrap 5 is installed, either as a Ruby gem or using CDN or packagemanager or git submodule of the sass:

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
```


Add this line to your application's Gemfile:

```ruby
gem "simple_form"
gem "devise-bootstrap-views", github: 'asecondwill/devise-bootstrap-views'
```

And then execute:

    $ bundle install

## I18n

Install [devise-i18n](https://github.com/tigrish/devise-i18n) for other locales. Make sure to insert `gem 'devise-i18n'` before `gem 'devise-bootstrap-views'`, see [#55](https://github.com/hisea/devise-bootstrap-views/issues/55).

## Customizing Views

The `devise:views:bootstrap_templates` generator will copy all views to your application, so you can modify the files as you wish:

```sh
$ rails generate devise:views:bootstrap_templates
```

The password eye feature requires the stimulus component:

 `pin stimulus-password-visibility`

 and follow the [instructions](https://www.stimulus-components.com/docs/stimulus-password-visibility/)

## Contributing

1. Fork it ( https://github.com/hisea/devise-bootstrap-views/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
