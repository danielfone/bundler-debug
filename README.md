Demonstration of bundler resolver issues with .gemspecs. Gems are:

* 'rails', '~> 3.0'
* 'capybara', '~> 2.2.0'

`bundle --gemfile Gemfile.success` should succeed

`bundle --gemfile Gemfile.failure` should also succeed, but will fail.

bundle_resolver.log is the output of `DEBUG_RESOLVER=1 bundle --gemfile Gemfile.fail`.
