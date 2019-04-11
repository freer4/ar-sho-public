---
layout: codex
permalink: /codex/index.html
title: Tau Codex Supplement | WH40K 8th Edition
navtext: Codex Home
description : Rules for the Ar'sho Enclave, a fan-crafted Tau sept choice based on the Warhammer 40,000 8th Edition Tau Codex.  
hero: "/assets/images/greatergood_stuarthughe.jpg"
heroalt: "Greater Good courtesy of jeffszhang"
---

# Tau Codex Supplement

## Rules for Warhammer 40,000 Armies 

Built around 8th Edition Warhammer 40,000 and its Tau Codex. Any "C" value in a datasheet refers to the [official Codex available here](https://www.games-workshop.com/en-US/Codex-Tau-Empire-2018-ENG)

---

This is a fan-made Sept and should not be considered official in any capacity (*yet...*). We strive to keep the rules here balanced - this is not intended to be some sort of cheese army filled with supermen. Please feel free to utlize the comments section on each page to provide your feedback or start a discussion! 

## Stats

##### Models

{% include statheader.html row=site.data.wargear.Models.Aunsahe %}
{% for wargear in site.data.wargear.Models %}|{% assign props = wargear | last %}{% for prop in props %}{{prop | last}}|{% endfor %}
{% endfor %}

##### Wargear

{% include statheader.html row=site.data.wargear.Weapons.BurstRailRifle %}
{% for wargear in site.data.wargear.Weapons %}|{% assign gearid = wargear | first %}{% assign props = wargear | last %}{% for prop in props %}{% assign propname = prop | first %}{% assign propval = prop | last %}{% if propname == "Weapon" and site.data.wargear.Linked contains gearid %}[{{propval}}](/codex/Wargear/{{propval | replace: " ", "_"}}.html){% else %}{{propval}}{% endif %}|{% endfor %}
{% endfor %}

##### Support Systems

{% include statheader.html row=site.data.wargear.SupportSystems.MarkerlightAnalysisSystem %}
{% for wargear in site.data.wargear.SupportSystems %}|{% assign props = wargear | last %}{% for prop in props %}{{prop | last}}|{% endfor %}
{% endfor %}

---

## Point values

##### Models

| Model | Points |
|:---|:---:|
{% for wargear in site.data.wargear.Models %}{% assign props = wargear | last %}{% assign iden = wargear | first %}|{{props.Unit}}|{{ site.data.wargear.Points[iden] }}|
{% endfor %}

##### Weapons

| Item | Points |
|:---|:---:|
{% for wargear in site.data.wargear.Weapons %}{% assign props = wargear | last %}{% assign iden = wargear | first %}|{{props.Weapon}}|{{ site.data.wargear.Points[iden] }}|
{% endfor %}

##### Support Systems

| System | Points |
|:---|:---:|
{% for wargear in site.data.wargear.SupportSystems %}{% assign props = wargear | last %}{% assign iden = wargear | first %}|{{props.Name}}|{{ site.data.wargear.Points[iden] }}|
{% endfor %}
