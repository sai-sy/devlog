---
title: "Auto Directory Hell"
date: 2023-01-15T06:49:00-05:00
draft: false
projects:
- devlog
---
### Where I left off:
This theme is beautiful, but I can't for the life of me get the side bar to register each project as it's own heading. I want to seperate my posts please please please please please
### Where I thought we ended:
The sidebar works and I can add different projects to it now. I think next time I'm gonna work on hosting since this site is pretty much done. The beauty of GO, Markdown, and auto directory systems is beautiful. I love auto directory.
### Where we end:
I am too tired. This journey, this single leg of the ever long journey, has drained me thourougly. Apparenly the side bar section only works with the 'Projects' header and `/projects` directory. I want to be able to organize them all by each individual project. I have submitted the github issue. I shall now rest in my travellers cot (my bed with mattress and blankets and pillows). Goodnight(its literally morning I worked a 9pm to 3am before this) reader

### The Journey:
#### 7:02 AM  
I like this format of left off, ending, then journey. I think I'm gonna go with this. Okay so this poison theme is great and it's the best doc looking theme with support for multiple blogs under `./content`. I'm following the github docs (very well made) and for some reason it refuses to let me add more side bar options even when I create './content/projectName/post' it doesn't show up. I update the `.config.toml` to include the path to the directory and yet it doesn't work

I also can't rlly figure out how multiple windows works in NVIM and how to properly open my terminal so I have like 3 different windows of WSL open so that's fun
#### 7:10 AM
{{< tabs tabTotal="2" >}} 

{{% tab tabName="First Tab" %}}
Woah I can do tabs
{{% /tab %}}

{{< tab tabName="Second Tab" >}}
{{< highlight text >}}
I still can't make the damn side bar work and its pissing me off
{{< /highlight >}}
{{< /tab >}}

{{< /tabs >}}

#### 7:25
I did it!!!! Maybe I shouldn't be doing work at 7 in the morning after a night long club shift. But my only problem was my meta data in my posts was making every post a draft instead of public. I'm fuming. But I learned a couple things
1. nvim has not made me any faster and I believe with the speed of electron apps, extensions, and knowing your keyboard shortcuts, VSCode is just as good for me. Although I will stick with nvim because it's fun feeling elitist and better
2. My WSL experience is disgustingly slow in `/mnt/c/.....` and will need to find a better solution for having my work available on my windows side and my ubuntu root
3. docs have typos too. proof read before making github issues

### TODO
- [x] make first post  
- [ ] make a home page to view all posts in reverse chronological  
- [x] make the side bar organized by projects  
- [ ] have an svg of my signature at the bottom of each post  
- [ ] have this todo list a part of the theme for each post but then have it dynamically update as i change  
- [ ] have the date in each post 
- [ ] maybe have an auto filter system to censor swear words as I post. I want to be raw and expressionate in these posts but also ion need employers and such seeing me chat mad shit in the most vulgar language I can spew out at 3:30 in the morning while I'm struggling
