<div align="center">
  <a href="https://www.simonstalenhag.se/">
    <img alt="eth logo" src="https://pbs.twimg.com/media/FNVLDsdWUAE_SOW?format=jpg&name=large" >
  </a>
  <p align="center">
    <a href="https://github.com/LuozhuZhang/NorthBound-Trace/graphs/contributors">
      <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/LuozhuZhang/NorthBound-Trace">
    </a>
    <a href="https://GitHub.com/LuozhuZhang/NorthBound-Trace/issues/">
      <img alt="GitHub issues" src="https://badgen.net/github/issues/LuozhuZhang/NorthBound-Trace/">
    </a>
    <a href="http://makeapullrequest.com">
      <img alt="pull requests welcome badge" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat">
    </a>
  </p>
</div>

# Load the Data

<img width="1105" alt="Screen Shot 2022-05-04 at 17 42 43" src="https://user-images.githubusercontent.com/70309026/166658463-7cd3e9e8-645a-4d8d-989f-789252e2ddf1.png">
<img width="1105" alt="Screen Shot 2022-05-04 at 17 43 19" src="https://user-images.githubusercontent.com/70309026/166658557-e939932e-e7a9-49b1-97f4-b48c916a32cc.png">

# Simple Analysis
<img width="1112" alt="Screen Shot 2022-05-04 at 17 45 10" src="https://user-images.githubusercontent.com/70309026/166658916-f22daaaf-46d7-4ab2-af79-3807e8ed7bd3.png">
<img width="1097" alt="Screen Shot 2022-05-04 at 17 45 22" src="https://user-images.githubusercontent.com/70309026/166658948-682353ac-1e02-4e9a-823b-f079d70245c1.png">
<img width="1101" alt="Screen Shot 2022-05-04 at 17 45 35" src="https://user-images.githubusercontent.com/70309026/166658971-67755b69-0d99-4bd3-8839-16ec100b23f4.png">
<img width="1099" alt="Screen Shot 2022-05-04 at 17 45 46" src="https://user-images.githubusercontent.com/70309026/166659002-ada180a7-6613-46cc-b0d1-fcb204bdf002.png">
<img width="1101" alt="Screen Shot 2022-05-04 at 17 45 56" src="https://user-images.githubusercontent.com/70309026/166659032-2cb18b87-75ac-4e64-9449-c0be93c7e357.png">

# Investment Strategy
Constructing Bollinger Band timing strategy based on northbound capital change data can effectively judge the short-term rise and fall of the market

As for whether northbound funds have an indicative role, we can observe through the backtesting performance of the timing model. To this end, we construct a Bollinger Band strategy based on the inflow scale data of northbound funds:

* (1) When the scale of northbound capital inflow on that day > the average value of northbound capital in the past 252 trading days + 1.5 times the standard deviation, then buy CSI 300 across the entire position;

* (2) When the scale of northbound capital inflow on that day < the average value of northbound capital in the past 252 trading days - 1.5 times the standard deviation, the position will be cleared and sold CSI 300;

* (3) Measured by buying at the opening price of the next day.
<img width="1108" alt="Screen Shot 2022-05-04 at 17 47 49" src="https://user-images.githubusercontent.com/70309026/166659325-4aafa4d3-66f7-4315-bf16-e14fdc84af26.png">

Evaluate the investment strategy
<img width="1105" alt="Screen Shot 2022-05-04 at 17 48 40" src="https://user-images.githubusercontent.com/70309026/166659468-e37e8d86-a169-4449-a38c-cff403894e92.png">
<img width="1107" alt="Screen Shot 2022-05-04 at 17 49 03" src="https://user-images.githubusercontent.com/70309026/166659526-5065933f-1620-49ff-b9a2-cecf2d9ee8fc.png">

# Backtesting

<img width="1109" alt="Screen Shot 2022-05-04 at 17 49 39" src="https://user-images.githubusercontent.com/70309026/166659604-1d236bcf-92fe-44f8-ac27-390a9b52cac6.png">
<img width="1105" alt="Screen Shot 2022-05-04 at 17 49 49" src="https://user-images.githubusercontent.com/70309026/166659620-65eb86c0-8f63-41ac-b8bf-94c7dd1a30b4.png">
<img width="1105" alt="Screen Shot 2022-05-04 at 17 50 00" src="https://user-images.githubusercontent.com/70309026/166659656-7854c092-12ea-4fad-aa6d-d2dfeff352da.png">

I believe data can give us the truth, but value capture relies on creation and growth, not a zero-sum game

I don't want to be swallowed by a sudden tsunami while I'm swimming

# Reference
[1] : 《Evidence-Based Technical Analysis》 and [TSSB](http://tssbsoftware.com/) - David Aronson

[1] : 《Testing and Tuning Market Trading Systems》 - [Timothy Masters](http://www.timothymasters.info/home.html)
