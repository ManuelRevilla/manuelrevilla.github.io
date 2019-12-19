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

<center>
<strong>&middot; Why I started my website/blog &middot;</strong> 
</center>


I wanted to start by telling you why I created this blog, what you will be seeing more of in my posts, and my overall experience of creating my website.

Since I started in academia, I have witnessed the emergence of huge amount of vias to share and disseminate our scientific contributions to an specific area of knowledge and the general public. All of them, to a greater or lesser extent, fulfill their purpose. But sometimes we miss out on valuable information among the wide range of communication channels available. That's why I decided to create this website as an official way of communication, an make you easier to know more and more about my professional progession as a researcher.  


<center>
<strong>&middot; First of all, I apologize &middot;</strong> 
</center>


English writing has never been a strong suite of mine and I will tell you, I am no expert on any of this. I try to be a "perfectionist" but I am nowhere near perfect. I figure it will be a lot of trial and error so please bear with me on any grammar/spelling mistakes. 


<center>
<strong>&middot; Enjoy the experience of building your own website/blog &middot;</strong>
</center>


After being inspired to start my website/blog, I wanted to create them in a professional way and would allow me to make updates in a simple and fast way. I could have gone to a web designer, but in that case I would have lost the experience of creating on my own. Taking advantage of my skills in <a href="https://www.r-project.org/" target="_blank">R</a> environment, I decided to built it using <a href="https://rstudio.com/" target="_blank">RStudio</a> open-source. As a researcher I am used to work programming in R to perform statistical and data analysis, so why not develop my own website using this language and have fun throughout the entire process... This means I would be able to maintain my website in R, have a lot more flexibility and control over the look of my website.

In the next lines I summarize the steps I follow to create my website. For a more detail guideline you can consult the extremely helpful <a href="https://alison.rbind.io/post/2017-06-12-up-and-running-with-blogdown/" target="_blank">blog of Alison Hill</a>.


<ol style="list-style-type: decimal">
  <li>
    Setting up <a href="https://pages.github.com/" target="_blank">GitHub Pages</a>:
  </li>

    <ul>
      <li>
         Create a GitHub account
      </li>
      <li>
        On your dashboard, create a New Repository (your_username.github.io)
      </li>
      <li>
        Create a local copy of this repository
      </li>
    </ul>
</ol>


<ol style="list-style-type: decimal" start="2">
  <li>
    Launch RStudio and create a New Project. Navigate to the folder above the working directory you just created from GitHub.
  </li>
</ol>


<ol style="list-style-type: decimal" start="3">
  <li>
    Install <a href="https://bookdown.org/yihui/blogdown/" target="_blank"> <code>blogdown</code> </a> package in your RStudio console:<pre><code class="hljs sql">## Install from CRAN
install.packages("blogdown")
## Or, install from GitHub
if (!requireNamespace("devtools")) install.packages("devtools")
devtools::install_github("rstudio/blogdown")</code></pre>
  </li>
</ol>


<ol style="list-style-type: decimal" start="4">
  <li>
    Install <a href="https://gohugo.io/" target="_blank">Hugo</a> using the <a href="https://bookdown.org/yihui/blogdown/" target="_blank"> <code>blogdown</code></a> package helper function:<pre><code class="hljs sql">blogdown::install_hugo()
# or
library(blogdown)
install_hugo()</code></pre>
  </li>
</ol>


<ol style="list-style-type: decimal" start="5">  
  <li>
    Build your site by choosing the <a href="https://themes.gohugo.io/" target="_blank">Hugo themes</a> that you like the most. If you belong to the academia field, <a href="https://themes.gohugo.io/academic/" target="_blank">Hugo Academic Theme</a> could be a good choice, this theme offers all the sections present in a standard <i>curriculum vitae</i> with a clean simple interface:<pre><code class="hljs sql"># create a new site with the academic theme
blogdown::new_site(theme = ".../hugo-academic", theme_example = TRUE)</code></pre>
  </li>
</ol>


<ol style="list-style-type: decimal" start="6">
  <li>  
    Configurate and customizate according your personal preferences. A complete guideline for the Hugo Academic theme can be find <a href="https://sourcethemes.com/academic/docs/customization/" target="_blank">here</a>. Running locally <code>blogdown:::serve_site()</code> in your RStudio project is especially useful as you can inmediately see the changes you have perform. If you would like to have Google monitor the analytics for your site so that you can study traffic flow on your pages, you will need to enable <a href="https://marketingplatform.google.com/intl/com/about/analytics/" target="_blank">Google Analytics</a>. First, sign up <a href="https://accounts.google.com/signin/v2/identifier?service=analytics&passive=1209600&continue=https%3A%2F%2Fanalytics.google.com%2Fanalytics%2Fweb%2F%3Futm_source%3Dmarketingplatform.google.com%26utm_medium%3Det%26utm_campaign%3Dmarketingplatform.google.com%2Fabout%2Fanalytics%2F%23&followup=https%3A%2F%2Fanalytics.google.com%2Fanalytics%2Fweb%2F%3Futm_source%3Dmarketingplatform.google.com%26utm_medium%3Det%26utm_campaign%3Dmarketingplatform.google.com%2Fabout%2Fanalytics%2F&flowName=GlifWebSignIn&flowEntry=ServiceLogin" target="_blank">here</a>. It will generate a tracking code for you. Enter the tracking code into <code>config.toml</code>
  </li>
</ol>


<ol style="list-style-type: decimal" start="7">
  <li>
    Link or host your local repository on your GitHub repository. For default your website domain will be (https://your_username.github.io/). If you want to set up a custom domain for your personal domain, in my case I buy www.manuel-revilla.com, you can purchase one in <a href="https://domains.google/" target="_blank">Google Domains</a>, is a very straightforward process. After that you can set up the custom domain for your website following the instructions of the <a href="https://help.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site" target="_blank">GitHub documentation</a>.
  </li>
</ol>


<ol style="list-style-type: decimal" start="8">
  <li>
    Last but not least, show your personal website to the World ;)
  </li>
</ol>


```
Very breef summary of the esencial steps to build your personal website:

- [x] Web: GitHub         | Create an account using GithHub Pages
- [x] RStudio             | package needed: "devtools", "blogdown" and "hugo"
- [x] RStudio             | Configurate and customizate your website
- [x] Web: GitHub         | Link or host your local repository (https://your_username.github.io/)
- [ ] Web: Google Domains | Buy and set up your personal domain
```


<blockquote>
  <p>
Please feel free to always share your advice and communicate with me along the way!
  </p>
</blockquote>

