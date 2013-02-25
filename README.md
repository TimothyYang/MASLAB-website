#MASLAB Website Guide (maslab.mit.edu)
###Tim Yang (timyang at mit.edu) 
###February 25, 2013 
---
For MASLAB 2013, I completely rewrote the MASLAB website. This document is a short overview of the site. Feel free to email me if there are any questions.

###Contents:

**1.** Links
**2.** How to Edit
**3.** Setup Overview
**4.** Notes

---

###Links:

**Old site**: http://maslab.mit.edu/2013/old_site/maslab.php

**New site**: http://maslab.mit.edu/2013/site/index.html

**Github**: https://github.com/TimothyYang/MASLAB-website/ 
(Note: this is current as of 12/29/13. The github repo is not synced with the server and may be behind. It’s mostly for browsing/referencing.)

---

###How to Edit:

**1.** Get access to the 6.816 athena locker. Ask the director or someone else with permissions.

**2.** On Athena (or Athena ssh), cd into 6.816

**3.** <notextile>The website is in 6.816/web_scripts. Each year keeps its website in a new folder, with that year’s name. The current site is in 6.816/web_scripts/2013/site. </notextile>

**4.** Edit the files directly.

---

###Setup overview:

Currently, the site is static, with largely CSS, HTML and a sprinkle of JS. 


The directories are:

  css		    holds css files

  files 		holds pdf or other files

  img		    holds image files

  includes 	holds re-used html files, such as the navbar and footer (see below)

  js		    holds js files, currently 
  
---

###Notes:

**1.** The site is built on Bootstrap (http://twitter.github.com/bootstrap/). Technically, the site is responsive, but the mobile version of the website has a lot of room for improvement.

**2.** Right now, the site loads the navigation bar (navBar) and footer through a super hack method with Javascript and HTML. Each page has a script called loadNavbar() and loadFooter() in its head which gets HTML from the includes folder and loads them into the appropriate divs. Typically, reusable components are included with PHP. However, this would be the only use of PHP in the site, so I didn’t want to spend time with PHP. Also, scripts should be in their own individual files.

**3.** Speaking of PHP, you’ll notice that the registration page has no registration form, because registration already passed. The old form is in PHP. To make a registbuttration form, you can either set up PHP and use the old form, or just use a Google Form/other established tool. I would use the latter because it’s easier, but both work.

**4.** As far as I know, there’s no version control for the old or current website. I would download a local copy, make changes, and upload the changed files. You can set up version control if you so feel.

**5.** The website currently uses Google Analytics for web traffic information. Quite frankly, we don’t really need analytics for this small site, but it’s fun to have (46% of visitors use Chrome, hooray!) 

**6.** The buttons on the front page all point to rules. Consider updating the content and links.

**7.** Consider updating the HTML/CSS files to match Google’s style guides http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml.

---

That’s all that I can think of for now! If you have any questions, contact me at timyang at mit.edu.

Best,
Tim
