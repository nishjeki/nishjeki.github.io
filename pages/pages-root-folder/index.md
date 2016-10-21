---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "Blog & Portfolio"
  url: 'http://nishjeki.github.io/blog/'
  image: widget-1-302x182.jpg
  text: 'When I get stucked and google is not able to find the solution, then I solve it and write a blog here.  I write about software development and sometimes other stuffs.  Thanks for visiting my blog, have a look around.'
widget2:
  title: "Software developments"
  url: 'https://github.com/nishjeki'
  image: widget-2-302x182.jpg
  text: 'The softwares which I am working on are open-source and available on <em>github.com</em>. Feel free to join in.'
widget3:
  title: "Meditation experiences"
  url: 'https://en.wikipedia.org/wiki/Meditation'
  image: widget-3-302x182.jpg
  text: 'In 2014 I started meditation on a regularly basis.  There were quite unrealistic experiences I had, but then I got a lot busy with work and family.  Now I started it again and I thought to write it down. Keep a watch here.' 
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---