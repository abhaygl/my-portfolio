| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [visualizing debt](visualizing-government-debt) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Makeover Monday
In a world full of different data visualizations, not everyone is going to think of modelling data the exact same way. There's all sorts of graphs, maps, and designs that can be used to represent the same dataset. That's the premise of the journey I went on in this page. Join me for Makeover Monday, where I choose a visualization from a website or database and redesign it to tell the story a completely different way.

## 1. Choosing a Visualization
First, I needed to choose a visualization. [Makeover Monday](https://makeovermonday.co.uk/) has a vast number of graphs and charts from a variety of sources that people redesign. Though many of them were interesting, including a table looking at congressional staff earnings and a scrolling bubble plot examining the pay gap in US Soccer, I decided to choose a graph displaying the differences in the average price for 1GB of data in countries around the world. I chose it because every time I go to my parent's home country of India, I notice that the price of data is EXTREMELY low compared to the United States, and I've always wondered how other countries stack up compared to the US as well.

photo

## 2. Critiquing the visualization
Next, I examined the visualization for its benefits and drawbacks. I submitted a Google Form detailing my specific thoughts on the graphics, as seen below:

photo

## 3. Wireframe
After I disected the visualization that was, I started to draw up what it could be. I wanted the graph to be able to show a) the differences between gigabyte costs and b) how massive the difference was between the most and least expensive countries. I wanted to make it a lot simpler, so I decided to sketch up a bar graph and a treemap. I thought both of them would be effective at displaying a lot of information in a visually appealing yet legible way. Plus, I knew I wanted to use color, and this would allow me to do that.

photos

After drawing up both, I decided to go with a bar graph. The treemap was interesting, but I ran into the same issue conceptually where the numbers more similar to each other were not clearly larger or smaller than one another.

## 4. Testing the Solution

I discussed my plans with two groups of people. One group was 2 fellow college students my age. They went to different universities than mine and came from very different disciplines. There were two individuals I consulted independently, all students in their early 20s pursuing degrees in Compsci and Law respectively. The second group was 2 peers from my Data Visualization class. They were both slightly older than me, mid-20s, completing their masters degrees.

For each person I talked to, I followed the same script:
_- What is this graph about?_
_- What story do you think this graph is trying to tell?_
_- Who is this graph for?_
_- What information pops out to you?_
_- What information do you think about, but the graph fails to provide?_
_- What parts about the design do you like or not like?_

I showed them both the sketch and a mock-up I quickly threw together on tableau, pictured below:

photo

Here is a paraphrasing of all the feedback I recieved. I put emphasis on including notes that were either unique or specifics that came up multiple times.

_Law Student, early-20s:_
I can tell that the graph is meant to tell me about the cost of average data plans across countries. I like that the colors are indicative of the price. I feel like there's too much information on the screen. I think I'm meant to know about the biggest and smallest numbers, but scrolling between everything doesn't let me compare them. I don't know if I'd use this, but I can see how someone interested in the topic could make use of this.

_Compsci Student, early-20s:_
This graph is about how much 1GB costs in different countries. It's trying to tell me the differences in those prices. I think it's useful for stats people to visually see differences between data plans, I don't think any newspapers can use this. I wish i could see all the information on a map. Right now, all the countries are just names, my eyes glaze over. It definitely shows which numbers are bigger and smaller, but because I have to scroll, I can't really see them properly. If I take some time, it really sets in how much bigger the cheapest and smallest gigabyte costs are.

_Masters' Student, mid-20s:_
This is a much better visualization than the original. You can clearly see this is meant to be showing data plans in different countries. I can definitely tell the difference in price, I wish the bigger and smaller numbers were closer together. You could use the map feature on Tableau, that would be an effective way of displaying country information. I think the gradient from red to green looks nice, but it looks like it doesn't accurately reflect the range of prices. Maybe try a stepped color option.

_Masters' Student, mid-20s_
I like this better. I don't like the flags in the original, I think you should use a country map. Maybe have both a country map and a bar graph. Then you could see the overall trends and still see individual country statistics. I like it the transition from green to red, but is that mid-point accurate? What if you had a median or mean line that showed what we should be referencing when we look at the bars on the graph?

After reviewing all the feedback, I decided a couple things to change. First, was that people wanted a map. It made it easy to identify countries and what cost of data plan theyre associated with. Second, they didn't like to scroll. Third, they wanted to be able to tell the difference between high and low costs across countries easier; they saw the story of how the lowest data plans and the highest data plans were, but they had trouble identifying it. Finally, they liked the simple colors, but thought the current gradient wasn't representative of the wide range of data.

I also decided to see how other individuals tackled the data visualization on Makeover Monday. There seemed to be different graphs that addressed parts of my peers' critiques, particularly I saw one that used the map feature quite well. But they all lacked the colors I wanted, and many times they stuck with a singular graph for ALL the data, when I think the current data needed some more.

## 5. Building my solution

Implementing all of the suggestions from my peers and my original vision for the design, this was what I came up with.

<div class='tableauPlaceholder' id='viz1707257296474' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Z2&#47;Z2PHJ27JQ&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='shared&#47;Z2PHJ27JQ' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Z2&#47;Z2PHJ27JQ&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>
<script type='text/javascript'>
  var divElement = document.getElementById('viz1707257296474');
  var vizElement = divElement.getElementsByTagName('object')[0];
  if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1200px';vizElement.style.height='1527px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1200px';vizElement.style.height='1527px';} else { vizElement.style.width='100%';vizElement.style.height='727px';}
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>
