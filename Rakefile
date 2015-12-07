require 'bundler'
require 'rubocop/rake_task'

Bundler::GemHelper.install_tasks

task :test do
  Dir['test/*_test.rb'].each do |testfile|
    load testfile
  end
end

RuboCop::RakeTask.new

task default: %w( test rubocop )
