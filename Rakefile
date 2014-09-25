require 'time'

def get_day
    posts = Dir.entries("_posts")
    posts = posts[2, posts.length - 2]

    maxDay = 0
    posts.each do |item|
        day = /-day-(\d*)/.match(item)[1].to_i
        if day > maxDay
            maxDay = day
        end
    end

    maxDay
end

desc 'create a new post'
task :post do
    maxDay = get_day

    title = ENV['title']
    if !title
        print "Title: "
        title = $stdin.gets.chomp
    end

    title = "Day #{maxDay + 1} - #{title}"
    slug = title.downcase.gsub(/'/, '').gsub(/[^\w]+/, '-').squeeze('-').gsub(/^-|-$/, '')
    slug = "#{Date.today}-#{slug}"

    file = File.join(
        File.dirname(__FILE__),
        '_posts',
        slug + '.markdown'
    )

    tags = ENV['tags'] || 'blog'
    
    File.open(file, "w") do |f|
        f << %{---
layout: post
title: #{title}
date: #{Date.today}
tags: [#{tags.split(' ').join(', ')}]
time: 
---
}
    end

    puts "Created new post with slug \"#{slug}\""

    if ENV['editor']
        system "#{ENV['editor']} _posts/#{slug}.markdown"
    end
end

desc 'get current day'
task :get_day do
    puts get_day
end

desc 'publishes everything'
task :publish do
    system "git add -A"
    system "git commit -m \"Publish day #{get_day}\""
    system "git push"
end