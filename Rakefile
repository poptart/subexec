require 'bundler'
Bundler::GemHelper.install_tasks

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = 'spec/**/*_spec.rb'
end

desc "Benchmark"
task :benchmark do
  sh "ruby benchmark/run.rb"
end

task :default => :spec
