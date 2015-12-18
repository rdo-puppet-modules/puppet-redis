source 'https://rubygems.org'

# special dependencies for Ruby 1.8
# since there are still several OSes with it
if RUBY_VERSION =~ /^1\.8\./
  gem 'rspec-core', '~> 3.1.7'
  gem 'nokogiri', '~> 1.5.0'
end

puppetversion = ENV.key?('PUPPET_VERSION') ? "~> #{ENV['PUPPET_VERSION']}" : ['>= 3.2.1']
gem 'puppet', puppetversion

if puppetversion =~ /^3/
  ## rspec-hiera-puppet is puppet 3 only
  gem 'rspec-hiera-puppet', '>=1.0.0'
end

facterversion = ENV.key?('FACTER_VERSION') ? "~> #{ENV['FACTER_VERSION']}" : ['>= 1.7.1']

gem 'facter', facterversion

gem 'rake'
gem 'rspec'
gem 'puppet-lint', '>=0.3.2'
gem 'rspec-puppet', '>=0.1.6'
gem 'puppetlabs_spec_helper', '>=0.4.1'

gem 'beaker-rspec'
gem 'bundler', '<= 1.10.5'
gem 'vagrant-wrapper'
