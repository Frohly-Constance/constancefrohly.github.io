To make a change:
Create a markdown or html file on github
Go to Terminal
go to constancefrohly.github.io (the correct folder located in Documents) with :
$ cd Documents/constancefrohly.github.io 
It will hopefully work (because when I set up github, I did :
$ cd "Documents" + $ git clone https://github.com/Frohly-Constance/constancefrohly.github.io.git + $ cd constancefrohly.github.io
To make sure you are on the correct github branch (only PublishingSource will translate to public changes on the side) : 
$ git checkout PublishingSource                                              
To import the changes made online :
$ git fetch origin + $ git pull origin PublishingSource 
To push changes on the site, I think the command is: 
$ git push origin PublishingSource 



Old index.html file replace by index.md file:
```html
---
layout: default
---
<!DOCTYPE html>
<html>
<head>
    <title>Constance Frohly's Research</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="Research.md">Research</a></li>
        </ul>
    </nav>
    <p>Explore my academic research on the Research page.</p>
</body>
</html>
```



    {::comment} 
From _config.yml:
navigation:
  - title: About
    url: /
  - title: Research
    url: /research.html

    From index.md: 
{% include header.html %}
{:/comment}
