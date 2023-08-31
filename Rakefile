# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require 'rake'
require 'rspec/core/rake_task'

require 'cucumber'
require 'cucumber/rake/task'

require 'coveralls'
require 'coveralls/rake/task'
Coveralls::RakeTask.new
task :test_with_coveralls => [:spec, :cucumber, 'coveralls:push']

require_relative "config/application"

Cucumber::Rake::Task.new
RSpec::Core::RakeTask.new

Rails.application.load_tasks
