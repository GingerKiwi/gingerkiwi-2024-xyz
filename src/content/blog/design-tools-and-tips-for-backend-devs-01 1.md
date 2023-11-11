---
title: "Design Tools and Tips for Backend Developers - Part 01: Finding Design Files and Figma to Code 101"
date: 2023-08-08
tags:
  - post
  - featured
  - design
  - css
  - figma
  - backend
  - tools
  - tips
description: This is the first in a series of articles on tips and tricks for web and app design - both for backend dev, and new developers. Every time I get in a discussion with backend or sometimes full-stack devs that prefer the backend, they say that one reason they prefer backend is that they're "not good at design". However, with a few simple tools and tips even those scared of design can become more comfortable in designing good looking apps. Today we're looking at where to find Figma design files and then how to quickly use them to get started coding.
---
Every time I get in a discussion with backend or sometimes full-stack devs that prefer the backend, they say that one reason they prefer backend is that they're "not good at design". But just like anyone can learn the basics of coding, anyone can learn the basics of design. With a few simple tools and tips, even those scared of design can become more comfortable in designing good looking apps. 

This is the first in a series of articles on tips and tricks for web and app design - both for backend dev, and new developers. Note that because this series is aimed at devs who are uncomfortable with design, a few of the methods, tools, and tips are ones that I wouldn't necessarily recommend to frontend developers or those with experience in other types of art and design  or non-Figma tools like Adobe Xd/Adobe CC or Sketch.

Today we're looking at where to find Figma design files and then how to quickly use them to get started coding. In future articles, colour themes/pallets, Figma to react code plugins, typography (fonts), and accessibility will be covered.

## Overview (If You're Just Skimming!)

1. Find free files in Figma:
	- Scroll down to see the links to suggested sites and if they're free or have a small fee.
	- Read the info for the ones you're interested in using - There's tips on how to best find what you're looking for.
2. Import Figma files into your Figma account
3. Use Figma's new dev mode to extract the code for each section/component
4. Keep reading this series for more design tools and tips including 
	- Fonts/typography, 
	- Figma plugins (e.g. Figma to react code), 
	- Colour themes, pallets,
	- Accessibility,
	- Layout - Demystifying CSS Grid and Flexbox
	- Basic design rules and how to follow them
## Part 01:  Finding Design Files and Figma 101 for Backend Devs

Does the following sound familiar? You have a great idea for an app, but have no idea where to start with the frontend. But it needs a frontend! So you cobble together some Bootstrap CSS, but it still doesn't look as cool as its functionality, the layout is weird, it's failing accessibility testing, and you're swearing at whoever invented CSS (Håkon Wium Lie).

This series is designed to give backend devs and new devs a helping hand with design - we're all part of the awesome global dev community after all! It's much easier to focus on coding if you have a starting point in the design of the frontend. We don't have to re-invent the wheel to get coding and end up with great looking and well functioning app. With an already created Figma file and just 15 minutes of getting to know how to use Figma files you can go back to focusing on the fun puzzle of getting your app working and doing something!
### Where to Get Figma and Other Design Files

Figma files are a great place to start - especially with the newer developer mode that writes the majority of the CSS for us. But where can you get Figma files? Here's a few places that are either free or have a small fee. For the ones with a fee the listed fee is current as of August, 2023.
#### Figma Community

The Figma Community has thousands of free files. There's a wide variety of themes, styles, and apps including dashboard, landing pages, blogs, social media apps, and more. With such variety and so many files it can take some time to find something that matches the needs for your app.

Cost: Free - need to filter your search to only show free files.
Link: [https://www.figma.com/community](https://www.figma.com/community)
Link to free web design files (includes mobile and desktop): [ https://www.figma.com/community/tag/web/files](https://www.figma.com/community/tag/web/files)
#### UI Store Design

UI Store Design has over 650 free design files, with many of them being Figma files. Downloading is a two step process, because the site is at least partially funded by advertising. For now, make sure that the design you want to use has a Figma option. Some are only Sketch, Adobe Xd/Adobe CC, InVision, or Webflow. Later in this series I'll show you options to open Adobe Xd and Sketch files in Figma.

Cost: Free
Links:
	Apps: [https://www.uistore.design/categories/apps](https://www.uistore.design/categories/apps)
	Landing pages: [https://www.uistore.design/categories/landing-pages]( https://www.uistore.design/categories/landing-pages)
	Dashboards: [https://www.uistore.design/categories/dashboards]( https://www.uistore.design/categories/dashboards)
#### Frontend Mentor

While Frontend Mentor has many free challenges, you must be a paid monthly or annual member to download the Figma files. However, a paid membership comes with support from their Discord community as well as project requirements. It's a great place to start building full-stack apps for your portfolio if you need ideas of what to build. Projects can be filtered by difficulty level, language/tools (html, css, javascript, api), and free/paid.

- Link: [https://www.frontendmentor.io](https://www.frontendmentor.io)
- Cost: 
	- $12 USD for 1 month
		- 2x premium challenge Figma files
		- 5x free challenge Figma files
	-  $96 USD per year
		- Unlimited challenges with all Figma files
#### iCodeThis

iCodeThis is a newer daily frontend coding challenge site. It's a great option to get design ideas for components and simple pages. A membership is required to have access to the Figma files. But all memberships are a one fee for a lifetime membership, so it's a great option if you're frequently stuck. It's also a great option if you want to improve your css/UI engineering skills a bit at a time and enjoy doing coding challenges. You could even build small backends for some of the challenges where it makes sense like login screens, dashboards, and forms.

- Link: [https://icodethis.com/pro](https://icodethis.com/pro)
- Cost: 
	- Free - viewing the design of the day. Figma file isn't included.
	- $24 (current -) for lifetime "bronze" membership - get the past 14 days of coding challenges with Figma Files
	- $79 (current) for lifetime "silver" membership - get all coding challenges (currently 250+) with Figma files 

### The Basics of How to Import and Use Figma Files

Figma is a powerful design tool, so it can be overwhelming to get started if you don't have a design background. However, with a quick tour and about 15 minutes it's fairly straightforward to learn the basics of using already completed Figma files.

#### Importing Figma Files

Some Files will give you the option to "Open in Figma". For those files you can just click "Open in Figma". Other files require you to download them. In that case, use the four steps below.

The first step in using Figma files is importing them.
1. Open Figma - you may have to sign in in your browser
2. Go to your home - the small house icon in the upper left hand corner, below the menu bar
3. On the top right of the screen click on the "import" button. It's next to the "+ Design file" and "+ Fig Jam board" buttons.
4. When the dialog box says the file is imported, click "done", then double click your file to open it.
#### Export Assets Including Images and Icons

Did you know that you can export all of the assets in bulk? It's a great shortcut if you want to get coding as quickly as possible.

Before you do a bulk export:
 - Click outside of any of the frames/ designed screens to make sure that you haven't selected anything.
 - It's also good to check on the right hand side of the UI that your units are set to "rems" and not "pixels", though this is not required for a bulk export.

1. In the upper left hand corner, click on the down arrow next to the Figma "F" logo.
2. Choose "file", then "export".
3. A list of assets, including entire frames will show on the screen. All assets will have a green checkmark beside them. For now don't worry about which assets you might not need. Just export all of them.
4. Note: Assets with duplicate names will/ should be renamed by your OS.
#### Extracting the CSS / Code in Figma Dev Mode 

Figma has a new dev mode that takes the guessing out of using a Figma file, puts units in rems instead of pixels, and makes things much quicker. It even extracts the CSS code for you. We'll also take a look in a later article on how to use a plugin to extract React and CSS directly to Code Sandbox or downloaded to your local machine.

1. Make sure you have Dev mode enabled by toggling on the toggle with "</>" in the upper right hand corner
2. Select a frame (page) in the design
3. Information about that page including size in rem, background colour, and if there's any padding or margins is displayed in a graphic on the left-hand side.
4. Once you've made a note of the page design, continue to click on individual elements to get their size, colours, and typography (font). You can copy and paste from Figma into your repo.
	1. For example the following code is copied from a heading in the "Sunnyside Landing Page" from Frontend Mentor.

```css
color: #FFF;
text-align: center;
font-family: Fraunces 9pt Soft;
font-size: 3.5rem;
font-style: normal;
font-weight: 900;
line-height: normal;
letter-spacing: 0.54688rem;
text-transform: uppercase;
```

5. Go through the design one element at a time on each page to get the css. 
6. For measurements that have more than 2 decimal points, just round up or down to the closest. For example letter spacing of 0.54688rem becomes 0.55 rem.
7. You will still have to figure out the layout with css grid, flexbox, or a combination of the two. Don't worry there will be at least one future article on that.
## Congratulations You've Taken the First Step!

If you've made it this far you're well on your way to quickly finding and using designs so you can focus on coding. This is just a start, but it's a much quicker way to have a great design than muddling through from scratch. Keep reading this series for more design tools and tips for backend developers!
### Next in This Series:

- Colour Themes, Tools, and Tips
- Typography and Fonts 101
- 7 Basic Design Rules and How to Apply Them
- Accessible Design - A11y in App Design
- Layout - Demystifying CSS Grid and Flexbox
- Photos, Images, and Videos
- Quickly Using Figma for Wireframes
- Figma Plugins - Figma to React code and more.
- Using Figma to Mock out Designs
- Using Dev Mode in Figma