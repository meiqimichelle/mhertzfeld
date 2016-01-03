---
title: College Scorecard
layout: post-work
image:
 feature: college_feature.jpg
 title: Graduating college students
 credit: U.S. Department of Education
 creditlink: https://collegescorecard.ed.gov/
 work: college_work.jpg
author: Michelle Hertzfeld
tags: [code, gov]
categories: [work]
---
The Obama Administration had been trying to rank colleges for years, but coming to consensus on what 'good' means had proven too difficult. Instead, the [College Scorecard](https://collegescorecard.ed.gov/) provides data on student outcomes both as an easy-to-use online tool, and as an open-data API for others to make their own tools from.<!--more-->

As Lisa Gelobter put it in [her post on whitehouse.gov](https://www.whitehouse.gov/blog/2015/09/12/under-hood-building-new-college-scorecard-students), "this work was truly collaborative team effort, with teams from the Departments of Education and of the Treasury, White House Domestic Policy Council, Council of Economic Advisors, and Office of Management and Budget, the [General Services Administration’s 18F](https://18f.gsa.gov) and the [U.S. Digital Service](https://www.whitehouse.gov/digital/united-states-digital-service)."

She continues:

"We received direct input from students, families, and their advisers to provide the clearest, most accessible, and reliable national data on college cost, graduation, debt, and post-college earnings. This new College Scorecard can empower Americans to: rate colleges based on what matters most to them, highlight colleges that are serving students of all backgrounds well, and to focus on making a quality, affordable education within reach."

"For the first time, the public can access the most reliable and comprehensive data on students’ outcomes at specific colleges, including former students’ earnings, graduates’ student debt, and borrowers’ repayment rates. The data is also available for various sub-groups, like first generation and Pell students. Because the data will be published through an API, researchers, policymakers, and members of the public can customize their own analysis of college performance more quickly and easily."

**Read her entire post on what went into creating this site [here](https://18f.gsa.gov/2015/09/14/college-scorecard-launch/)**

### Coding the scorecard

For this project, I was one of two front end developers that worked over three months to bring the extensive user research and usability-tested designs to life. My role was primarily HTML/CSS. I made sure front end code was built to modern standards; was documented so that whoever took over the project could continue without problem; and was accessible and progressively-enhanced. Site accessibility was no small feat since the site design included custom versions of almost every form element available to a browser.

![College scorecard responsive views, homepage](/assets/img/college_responsive.jpg)

![College scorecard responsive views, results page](/assets/img/college_responsive-results.jpg)

One of my favorite parts of working on this project was the live styleguide we created to make sure our styles were modularizing the way we'd hoped, and not becoming too inter-mingled as to make long-term maintenance difficult. The images of the styleguide below also show some of our custom form elements.

![College scorecard styleguide](/assets/img/college_styleguide.jpg)

Although responsive design is always important on every project, user testing had shown that our front end tool (the interface at collegescorecard.ed.gov) in particular needed to be usabiliy on cellphone-sized screens. It turned out that our primary audience for that tool was much more likely to access the site on a mobile device than on a desktop computer. Conversely, when things got tight close to rollout, we spent less time on perfecting responsive work on the data downloads part of the site, as the users for that section primarily used full desktop computers.

One of the challenges of this project was the need to keep our work hidden behind passwords and logins until the President made the official announcement. This made testing things like meta tags challenging to say the least! Fortunately, since this project was meant to launch tons of newly-open data into the world, after the announcement our entire codebase (in addition to the College Scorecard API and data) was made open on GitHub for others to fork, learn from and improve.


### Press sampling

**NPR: [President Obama's New 'College Scorecard' Is A Torrent Of Data](http://www.npr.org/sections/ed/2015/09/12/439742485/president-obamas-new-college-scorecard-is-a-torrent-of-data)**

_"This is government working for us. My first thought was, 'Go Department of Education,' " says Sara Goldrick-Rab, who teaches education policy at the University of Wisconsin, Madison. "We had some information college by college before, but we didn't have most of these outcomes here."_

**The White House: [Weekly Address: A New College Scorecard](https://www.whitehouse.gov/blog/2015/09/12/weekly-address-new-college-scorecard)**

_"The President speaks about the launch of a new College Scorecard, meant to help students and parents identify which schools provide the biggest bang for your buck."_

**The Atlantic: [Obama's New College Scorecard Flips the Focus of Rankings](http://www.theatlantic.com/education/archive/2015/09/obamas-new-college-scorecard-flips-the-focus-of-rankings/405379/)**

_"Earlier this September, the president unveiled his much-anticipated “College Scorecard” as part of that pledge. The new tool, however, isn’t exactly a ranking system. Instead, it gives users access to extensive federal data on the student-debt and attendance-cost data for more than 7,000 U.S. higher-ed institutions allowing them to compare institutions; students can use the Scorecard to list and sort schools based on the institutions’ on-time graduation rates, school size, and salary after attending, among other factors."_

**The Huffington Post: [Roundup of news on the College Scorecard](http://www.huffingtonpost.com/news/obama-college-scorecard)**
