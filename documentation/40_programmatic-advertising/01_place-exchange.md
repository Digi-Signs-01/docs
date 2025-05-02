---
title: "Place Exchange"
slug: place-exchange
publish: false
date: 2025-05-03
update: 2025-05-03
description: Place Exchange
categories:
  - start
---

Place Exchange
==============

To ensure your Place Exchange credentials are correct, simply replace the **Org\_ID** and **Ad\_UnitID** and enter the URL in a browser:

```
https://api.placeexchange.com/v3/orgs/Org_ID/adunits/Ad_UnitIT/adrequests?format=vast4
```

If all is correct, the page should load a content that looks like:

```
1 <VAST xmlns="http://www.iab.com/VAST " version="4.0">
2 <Ad id="31d23e9b-aoab-ioc3-zkpd3-72237923237">
3 <InLine>
4 ...
5 </InLine>
6 </Ad>
7 </VAST>
```
