# frozen_string_literal: true

require "bundler/gem_tasks"
require "rspec/core/rake_task"
require "rubocop/rake_task"

RuboCop::RakeTask.new
RSpec::Core::RakeTask.new(:spec)

task default: :ci

task ci: %i[rubocop spec steep]

namespace :rbs do
  desc "Generate RBS files"
  task :generate do
    sh "rbs-inline", "--opt-out", "--output=sig", "lib"
  end
end

desc "Run steep type check"
task :steep do
  sh "bundle exec steep check"
end
