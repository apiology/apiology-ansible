require 'quality/rake/task'

Quality::Rake::Task.new do |t|
  t.skip_tools = %w(rubocop flog reek flay) # See quality gem issue #27
  t.verbose = true
  t.extra_files = ['playbook.yml']
end

task ci: :quality

task default: :ci
