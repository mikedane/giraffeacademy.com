---
date: 2017-11-15T17:52:37-05:00
title: "Getting Input From Users"
seo_title: "Getting Input From Users | PHP | Mike Dane"
subheader:
     greeting: PHP - Programming Language
     description: This course covers the basics of programming in PHP. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers getting input from users in PHP.
author: Mike Dane
image: getting-input-from-users.png
video: XZeFP-CXQj4
url: /web-development/php/getting-input-from-users/
weight: 10
---

## Code

{{< code lang="html" file="site.php">}}
<form action="site.php" method="GET">
     Username: <input type="text" name="username">
     <input type="submit">
</form>

<?php
     echo $_GET["username"];
?>
{{< /code >}}