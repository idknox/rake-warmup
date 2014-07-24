require "time"


desc "Shows current date/time"
task :time do
  puts "#{Time.new}"
end

desc "greets user"
task :greet do
  puts "What's your name?"
  g = STDIN.gets.chomp
  puts "Hello, #{g}"
end

desc "prints fav food env variable"
task :print_favorite_food do
  puts "Your favorite food is #{ENV["FAVORITE_FOOD"]}"
end

namespace :morning do
  task :get_dressed => :wake_up do
    puts "get dressed"
  end

  task :ready_for_class => [:wake_up, :eat_breakfast, :brush_teeth] do
    puts "get ready for class"
  end

  task :wake_up do
    puts "wake up"
  end

  task :eat_breakfast do
    puts "eat breakfast"
  end

  task :brush_teeth do
    puts "brush teeth"
  end

end

task :default => "greet"
