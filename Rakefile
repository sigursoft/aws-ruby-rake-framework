require 'yaml'
require 'rake/clean'

desc 'Default task'
task :default => [ :vpc, :bastion, :sns, :sqs, :ecs, :rds, :cloudfront ] do
  unless Dir.exist? 'workinprogress' then mkdir 'workinprogress' end
  unless File.exist? 'workinprogress/output.txt' then touch 'workinprogress/output.txt' end
  puts "I'm done!"
end

desc 'SNS task'
task :sns do
  puts "I'm building SNS topic!"
end

desc 'SQS task'
task :sqs do
  puts "I'm building SQS queues!"
end

desc 'CloudFront task'
task :cloudfront do
  puts "I'm building CloudFront!"
end

desc 'VPC task'
task :vpc do
  puts "I'm building VPC!"
end

desc 'Database task'
task :rds do
  puts "I'm building RDS!"
end

desc 'Bastion task'
task :bastion do
  puts "I'm building bastion host!"
end

desc 'ECS cluster'
task :ecs do
  puts "I'm building ECS cluster!"
end

task :clean do
 puts 'Cleaning the output'
 rm 'workinprogress/output.txt'
 rmdir 'workinprogress'
end
