---
layout: post
title:  "Stewdonyms"
date:   2019-12-08 12:30:10 +0530
categories: Blog
---
Thou hath always asked me, "O Mighty Shriram, wherefore doth thou beckon thy doggo with different names each day?".
Well there is a certain format to generating these names and indeed an algorithm which can list out all those names.
The format specifies that a valid name for stewie shall consist of consonant + accessory consonant + vowel + bridging consonant + 'y'(phonetic alphabet \\i\\ ).

All names that are not mentioned in these 1500 names are invalid and can only be made valid by permission on yours trule.

Namelist dump:

<script src="https://gist.github.com/notshriram/c23ec7e8c16bff66e34dc80b14da1e9f.js"></script>

You can check out the generator implemented in c++ here:

<script src="https://gist.github.com/notshriram/82f7d42112ce22ce6fa27e9bd1fc16e8.js"></script>


this snippet shows each part of the names:
{% highlight c++ %}
  std::vector<std::string>conso = { "p","b","m","t","d","n","k","g","f","s","j","sh","ch","h","" };
	std::vector<std::string>mixable = { "","r","l","w","y" };
	std::vector<std::string>vowel = { "a","e","i","o","u" };
	std::vector<std::string>tail = { "mb","mp","bb","pp" };
{% endhighlight %}

Finally, we can calculate that there are in total 15 x 5 x 5 x 4 valid names that can be generated.

Hope this helps,
ciao ciao!
