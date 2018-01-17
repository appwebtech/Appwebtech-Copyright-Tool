# Appwebtech Copyright Tool

<hr>
![](https://user-images.githubusercontent.com/13242902/35069768-1d932f58-fbd3-11e7-927c-af5bb82c4234.png)

As I was coding the [appwebtech](http://theappwebtech.com/) website, I ran into issues on how I can create a dynamic copyright tool which will update automatically when crossing a new year. I have been coding my web application since mid DEC to enable only partial view of the front-end when it goes live and I realised that much stuff pointed to 2017.

Anyways, Instead of using Javascript, I thought it wise to just build this ruby gem from scratch and make it available as a gem file on the [rubygems website](https://rubygems.org/).

Any developer can use this gem to personalise their web application as a Ruby construct, and later call it to view via the application layout using embedded ruby as below; 

```erb
.....
<%= yield %> 
<p> <%= @copyright %></p>
.....
```


## Installation

Add this line to your application's Gemfile:

```ruby
gem 'appwebtech_copyright_tool'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install appwebtech_copyright_tool

## Usage

```ruby
AppwebtechViewTool::Renderer.copyright 'Appwebtech ', 'All rights reserved'
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. 

In case I release a new version, I'll update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org). 

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/appwebtech/appwebtech_copyright_tool.

## Website and social media

[Appwebtech](http://www.theappwebtech.com/) website.

[Github](https://github.com/appwebtech) code page.

[Twitter](https://twitter.com/appwebtech) page.

[Facebook](https://www.facebook.com/appwebtech/) page.

[Pinterest](https://it.pinterest.com/appwebtech/) page.

[Linkedin](https://www.linkedin.com/company/appwebtech/) page.

 


## License


The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
