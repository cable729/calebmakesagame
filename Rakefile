require 'time'

desc 'create a new post'
task :post do
    title = ENV['title']
    tags = ENV['tags'] || ''
    slug = "#{Date.today}-#{title.downcase.gsub(/[^\w]+/, '-').squeeze('-')}"

    file = File.join(
        File.dirname(__FILE__),
        '_posts',
        slug + '.markdown'
    )

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
end