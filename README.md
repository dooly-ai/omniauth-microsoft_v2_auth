Please note that this is merely a fork of a sub-directory in [this example Ruby Microsoft Graph repo](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/master/omniauth-microsoft_v2_auth),
with the README tweaked to show how to install the gem directly from git (since it doesn't seem to
actually be published on RubyGems).

# Omniauth::MicrosoftV2Auth

Microsoft V2 OAuth2 Strategy for OmniAuth.
Can be used to authenticate with Microsoft Services and get a token for the Microsoft Graph Api.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'omniauth-microsoft_v2_auth', github: 'dooly-ai/omniauth-microsoft_v2_auth'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install omniauth-microsoft_v2_auth

## Usage

```ruby
Rails.application.config.middleware.use OmniAuth::Builder do
  provider :microsoft_v2_auth, ENV['AZURE_APPLICATION_CLIENT_ID'], ENV['AZURE_APPLICATION_CLIENT_SECRET']
end
```
