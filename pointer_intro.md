#পয়েন্টার কি?

সি ল্যাঙ্গুয়েজের একটি বেশ শক্তিশালী ফিচার হল পয়েন্টার। পয়েন্টার দিয়ে ফাংশনের ভেতর থেকে ভ্যারিয়েবল বা অ্যারে পাল্টানো, মেমোরি অ্যালোকেশন সহ বিভিন্ন অ্যাডভান্সড কাজ করা যায়। আমরা অ্যারের ব্যবহার দেখেছি আগের অধ্যায়ে। অ্যারের একটি বিষয় হল এটির সাইজ প্রথমেই বলে দিতে হয়, পয়েন্টার ব্যবহার করে আমরা চাইলে ডায়নামিক অ্যারে তৈরি করতে পারি যেটির সাইজ প্রোগ্রাম চলার সময়ে ঠিক হবে এবং সে অনুযায়ী মেমোরি অ্যালোকেটেড হবে।

পয়েন্টার কি বুঝতে হলে আমাদের বুঝতে কম্পিউটার মোমোরি কিভাবে কাজ করে। খুব সহজ করে বলতে গেলে বলা যায় আমরা যখন একটি ভ্যারিয়েবল ডিক্লেয়ার করি তখন সেটি মেমোরিতে একটি যায়গা নেয়। এরপরে আমরা ভ্যারিয়েবলে কোন ভ্যালু অ্যাসাইন করলে মেমোরির সেই নির্দিস্ট অংশে ভ্যালুটি সংরক্ষিত হয়। মেমোরির সাইজ, প্রাপ্যতা এবং অনেক বিষয়ের উপর ভিত্তি করে প্রতিবার প্রোগ্রাম এক্সিকিউট করলে এই ভ্যারিয়েবলের মেমোরিতে লোকেশন ভিন্ন ভিন্ন হয়। পয়েন্টারের কাজ হল মেমোরিতে এইসব ভ্যারিয়েবলের লোকেশন কে নিয়ে কাজ করা। আমরা পয়েন্টার দিয়ে মেমোরিরএইসব লোকেশনকে পয়েন্ট করতে পারি এবং চাইলে ওইসব লোকেশনের ভ্যলুগুলোকে নিয়েও কাজ করতে পারি। 

পয়েন্টার দিয়ে আমরা ডায়নামিক মেমোরি অ্যালোকেশন ছাড়াও স্ট্রিং বা অ্যারের উপর বিভিন্ন লজিকাল অপারেশন চালাতে পারি এবং ফাংশনের মধ্যেও ব্যবহার করতে পারি।
