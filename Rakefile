# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require 'coveralls'
Coveralls.wear_merged!('rails')

require 'rake'
require 'rspec/core/rake_task'

require 'cucumber'
require 'cucumber/rake/task'

require_relative "config/application"

Cucumber::Rake::Task.new
RSpec::Core::RakeTask.new


Rails.application.load_tasks
