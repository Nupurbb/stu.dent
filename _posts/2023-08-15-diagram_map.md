---
toc: true
comments: true
layout: post
title: interactive diagram
description: Look and click
type: tangibles
courses: { compsci: {week: 3} }
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Map</title>
</head>
<body>
    <h1>Click on the Map</h1>
    <img src="your-image.jpg" alt="Interactive Map" usemap="#map">

    <map name="map">
        <!-- Define clickable areas using the <area> element -->
        <!-- Example: Clickable rectangle -->
        <area shape="rect" coords="50,50,150,150" href="https://www.example.com/area1.html" alt="Area 1">

        <!-- Example: Clickable circle -->
        <area shape="circle" coords="250,150,50" href="https://www.example.com/area2.html" alt="Area 2">

        <!-- Example: Clickable polygon -->
        <area shape="poly" coords="350,50,400,100,300,100" href="https://www.example.com/area3.html" alt="Area 3">
    </map>
</body>
</html>


