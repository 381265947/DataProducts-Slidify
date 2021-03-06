---
title       : Data Products Course Project
subtitle    : 
author      : 381265947
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap, quiz]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

--- &radio

## Do you ever need to average lists of numbers?

1. _Yes!_
2. No

*** .hint
HINT: Everyone needs to average lists of numbers. All the time.

*** .explanation
People are always tossing around lists of numbers. What else would we do with them?

---

Hello. Let's talk about lists of numbers. Sometimes you have a list of numbers and you are desperate to average them. Well I've got a way for you to do that - along with visualizing the numbers. Does that sound like a great tool to have?

Well, enjoy: https://courseradude.shinyapps.io/project/

Github: https://github.com/381265947/DataProductsCourseProject

<img src="assets/img/dwarf.jpg" />

---

# Here's the code

Notice that spaces are handled properly because we live in the future.


```r
text <- "1, 2, 3, 4";
nums <- sapply(strsplit(text, "\\s*,\\s*"), as.numeric);
avg <- mean(nums);
avg;
```

```
## [1] 2.5
```

---  

# Here's the visualization


```r
plot(nums);
abline(h = avg);
```

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2.png) 
