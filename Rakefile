$:.unshift File.expand_path('../lib', __FILE__)
require 'routing_filter/version'
require 'rake'
require 'rake/testtask'

Rake::TestTask.new do |t|
  t.libs << 'lib' << 'test'
  t.pattern = 'test/**/*_test.rb'
  t.verbose = false
end

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "vigetlabs-routing-filter"
    gem.summary = %Q{Routing filters wraps around the complex beast that the Rails routing system is, allowing for unseen flexibility and power in Rails URL recognition and generation.}
    gem.description = %Q{Routing filters wraps around the complex beast that the Rails routing system is, allowing for unseen flexibility and power in Rails URL recognition and generation.}
    gem.email = "svenfuchs@artweb-design.de"
    gem.homepage = "https://github.com/vigetlabs/routing-filter"
    gem.authors = ["Sven Fuchs", "Brian Landau", "David Eisinger"]
    gem.add_dependency('actionpack')
    gem.version = RoutingFilter::VERSION
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: sudo gem install jeweler"
end

task :default => :test

