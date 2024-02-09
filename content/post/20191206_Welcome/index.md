---
title: Hello & Welcome to my first blog post
subtitle: Reasons to create a website

authors:
- admin

categories:
- R

date: 2019-12-06
math: false
diagram: false
markup: 
image:
  placement: 
  caption: ''
---

Welcome to the launch of my first website and my first blog post! My name is Manuel Revilla and I am so excited to share with you all my contributions to the scientific world gathered together in one website. The amount of ideas, how-to's and inspiration whirling around in my head is ready to jump out.  

{{< shortcodestarted >}}

I wanted to start by telling you why I created this blog, what you will be seeing more of in my posts, and my overall experience of creating my website.

Since I started in academia, I have witnessed the emergence of huge amount of vias to share and disseminate our scientific contributions to an specific area of knowledge and the general public. All of them, to a greater or lesser extent, fulfill their purpose. But sometimes we miss out on valuable information among the wide range of communication channels available. That's why I decided to create this website as an official way of communication, and make you easier to know more and more about my professional progession as a researcher.  


{{< shortcodeapologize >}}


English writing has never been a strong suite of mine and I will tell you, I am no expert on any of this. I try to be a "perfectionist" but I am nowhere near perfect. I figure it will be a lot of trial and error so please bear with me on any grammar/spelling mistakes.  


{{< shortcodeblog >}}

After being inspired to start my website/blog, I wanted to create them in a professional way and would allow me to make updates in a simple and fast way. I could have gone to a web designer, but in that case I would have lost the experience of creating on my own. Taking advantage of my skills in [R](https://www.r-project.org/ "R") environment, I decided to built it using [RStudio](https://rstudio.com/ "RStudio") open-source. As a researcher I am used to work programming in R to perform statistical and data analysis, so why not develop my own website using this language and have fun throughout the entire process... This means I would be able to maintain my website in R, have a lot more flexibility and control over the look of my website.

In the next lines I summarize the steps I follow to create my website. For a more detail guideline you can consult the extremely helpful [blog of Alison Hill](https://alison.rbind.io/post/2017-06-12-up-and-running-with-blogdown/ "blog of Alison Hill").  


1. Setting up [GitHub Pages](https://pages.github.com/ "GitHub Pages"):

  * Create a GitHub account
  * On your dashboard, create a New Repository (your_username.github.io)
  * Create a local copy of this repository

2. Launch RStudio and create a New Project. Navigate to the folder above the working directory you just created from GitHub.

3. Install [blogdown](https://bookdown.org/yihui/blogdown/ "blogdown") package in your RStudio console:
```
## Install from CRAN
install.packages("blogdown")
## Or, install from GitHub
if (!requireNamespace("devtools")) install.packages("devtools")
devtools::install_github("rstudio/blogdown")
```

4. Install [Hugo](https://gohugo.io/ "Hugo") using the [blogdown](https://bookdown.org/yihui/blogdown/ "blogdown") package helper function:
```
blogdown::install_hugo()
# or
library(blogdown)
install_hugo()
```

5. Build your site by choosing the [Hugo themes](https://themes.gohugo.io/ "Hugo themes") that you like the most. If you belong to the academia field, [Hugo Academic Theme](https://themes.gohugo.io/academic/ "Hugo Academic Theme") could be a good choice, this theme offers all the sections present in a standard *curriculum vitae* with a clean simple interface:
```
# create a new site with the academic theme
blogdown::new_site(theme = ".../hugo-academic", theme_example = TRUE)
```

6. Configurate and customizate according your personal preferences. A complete guideline for the Hugo Academic theme can be find [here](https://sourcethemes.com/academic/docs/customization/ "here"). Running locally ```blogdown:::serve_site()``` in your RStudio project is especially useful as you can inmediately see the changes you have perform. If you would like to have Google monitor the analytics for your site so that you can study traffic flow on your pages, you will need to enable [Google Analytics](https://marketingplatform.google.com/intl/com/about/analytics/ "Google Analytics"). First, sign up [here](https://accounts.google.com/signin/v2/identifier?service=analytics&passive=1209600&continue=https%3A%2F%2Fanalytics.google.com%2Fanalytics%2Fweb%2F%3Futm_source%3Dmarketingplatform.google.com%26utm_medium%3Det%26utm_campaign%3Dmarketingplatform.google.com%2Fabout%2Fanalytics%2F%23&followup=https%3A%2F%2Fanalytics.google.com%2Fanalytics%2Fweb%2F%3Futm_source%3Dmarketingplatform.google.com%26utm_medium%3Det%26utm_campaign%3Dmarketingplatform.google.com%2Fabout%2Fanalytics%2F&flowName=GlifWebSignIn&flowEntry=ServiceLogin "here"). It will generate a tracking code for you. Enter the tracking code into ```config.toml```


7. Link or host your local repository on your GitHub repository. For default your website domain will be (https://your_username.github.io/). If you want to set up a custom domain for your personal domain, in my case I buy [www.manuel-revilla.com](http://manuel-revilla.com/ "www.manuel-revilla.com"), you can purchase one in [Google Domains](https://domains.google/ "Google Domains"), is a very straightforward process. After that you can set up the custom domain for your website following the instructions of the [GitHub documentation](https://help.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site "GitHub documentation").

8. Last but not least, show your personal website to the World ;)
```
Very breef summary of the esencial steps to build your personal website:

- [x] Web: GitHub         | Create an account using GithHub Pages
- [x] RStudio             | package needed: "devtools", "blogdown" and "hugo"
- [x] RStudio             | Configurate and customizate your website
- [x] Web: GitHub         | Link or host your local repository (https://your_username.github.io/)
- [ ] Web: Google Domains | Buy and set up your personal domain
```


>Please feel free to always share your advice and communicate with me along the way!


