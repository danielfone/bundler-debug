Demonstration of bundler resolver issues with .gemspecs. Gems are:

* 'rails', '~> 3.0'
* 'capybara', '~> 2.2.0'

Gemfile.success has these dependencies directly. `bundle --gemfile Gemfile.success` will succeed.

Gemfile.failure references the .gemspec with these same dependencies. `bundle --gemfile Gemfile.failure` should also succeed, but will fail.

bundle_resolver.log is the output of `DEBUG_RESOLVER=1 bundle --gemfile Gemfile.fail`.
