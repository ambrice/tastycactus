require 'rubygems'
require 'nanoc3/tasks'

task :compile do
    system "rsync -rpgvP assets/ output"
    system "nanoc3 co"
end

task :release do
    system "rsync -a output/* ambrice@tastycactus.com:/home/ambrice/webapps/tastycactus/"
end

task :default => :compile
