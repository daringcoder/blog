---
layout: post
title: পাইথনে টেক্সট ফাইল রীড করা এবং ফাইল নিয়ে কাজ করা
---
প্রোগ্রামিং এ অনেক সময় বিভিন্ন টেক্সট ফাইল নিয়ে কাজ করতে হয়। যেমন: টেক্সট ফাইল তৈরী করতে হয় বা রীড করতে হয়। অামরা দেখব পাইথনে কিভাবে একটা টেক্সট ফাইলকে রীড করতে হয়। কোনো টেক্সট ফাইলকে ওপেন করার জন্য পাইথনে open() নামে একটা ফাংশন অাছে। অামি যেই ডিরেক্টরি থেকে পাইথন ইন্টারপ্রেটার চালু করেছি, সেই ডিরেক্টরিতে [names.txt](https://gist.github.com/Mehedi61/f4823ae3b7349a200d307fb42b013ede) নামে একটা টেক্সট ফাইল অাছে। এখন অামরা পাইথন দিয়ে ফাইলটাকে এক্সেস করব।
```python
names_file = open('names.txt', 'r')    # open the file named names.txt
>>>
>>> names = names_file.read()    # read the opened file and store in the names variable
>>>
>>> print(names)
Altaf, Anupa, Ahad, Miraz, Mehedi, Mohiminul, Misbah, Miftah, Shaker, Shakil, Salahuddin, Shihab, Israt, Nahid, Tania, Tarin, Taslib, Toheid, Shajid, Fahad, Faysal, Porimol, Sreekantha
```
