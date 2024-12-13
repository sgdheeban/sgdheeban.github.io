---
layout: post
title:  "My perspective on platforms evoltuion with the age of the company!"
date:   2024-12-10 14:49:30 -0800
categories: jekyll draft
---
- these are my perspective, my could be incomplete, if so, I might write a follow up post in the future with more experience
  - pls email if there is any counter thoughts, all views welcome
  - we cover these topics in this blog, because I believe these are small invisible, incosequential pebbles that comes in our way and endup becoming a roadblock to build complex systems
  - so much a note to self than others
  
- Platform is always there since day-1
- Frontend depends on distribution constrains - browser, tomorrow ai
- Backend evolves with the org 
- Architectures change, but principles don't
- Many perspectives on platform 
  - Engineers perspective architecture first
    - Architecture at different levels
      - Code level Clean Code, Solid principles or Domain Modeling
      - Software Systems level micro services, mono repos separation of concerns
      - Problem is this is a moving target, for ex. if you chose Rust, there is no OOPS
        - If you did OOPS it will make Rust unproductive, there is Hexagonal architectures
        - Tomorow there will be a new paradigm, as programming paradigms evolve, if not in 10 years, definitely in 30-50 years
      - My perspective is business first, technology exists to empower business
        - Think this is slightly more durable, until the nature of business changes, for ex, blockchain protocols or everything is AI or quantum
        - This means Performance first, Debuggability first
          - Performance has 2 characterstics - primary, business advantage, secondary - great engineers love it
      - Abstractions
        - If internal platform, keep wrappers thin & wide, aligned with open source, to keep debuggability high with the performance of open source
        - If you get enough scale to export this eventually, go to thicker wrappers like AWS, now with Coinbase Cloud, first web3 infra exporter
        - Don't start with heavy abstractions early on in startup life, because in startups tenures are shorters, heavy abstractions with no original developer brings the opposite effect, drag on the organization, low debuggability, degrading performance
      - Evolution of platform, don't optimize pre-maturely
        - Day 1 of a startup, your cloud functions are your backend platform
          - Be agile
        - 1-10 million business, your monorepo or simple medium coplex backend are your platform
          - Keep it simple
        - 10-100m+ business, your platform is complex enough to break down vertically to separate services, owned by teams
          - org reflects software structure or vice-versa
          - product infra there is a tussle between product management & engineering
            - manager roles becomes crucial
            - no silver bullets, reflects the DNA of the organization
        - 1B+ business, your platform has enough scale to break down common infra components to horizontal infra platform for entire company
          - surprisingly, this is less screwed up in retrospect across age of the company in my experience
            - may be engineers are seasoned when we come to this spot
          





You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
