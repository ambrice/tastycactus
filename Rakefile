require 'rubygems'
require 'nanoc3/tasks'

task :compile do
    system "rsync -rpgvP assets/ output"
    system "nanoc co"
end

task :default => :compile
