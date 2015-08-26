#পয়েন্টারের বেসিক অপারেশন

সি তে পয়েন্টারকে `*` দিয়ে লিখা হয়। আমরা যেভাবে ভ্যারিয়েবল ডিক্লেয়ার করি পয়েন্টারও সেভাবেই ডিক্লেয়ার করতে হয়। পয়েন্টারের ডেটা টাইপ হবে এটি যে ধরনের ভ্যালুকে পয়েন্ট করবে তার ডেটা টাইপ। পয়েন্টারে যেহেতু আরেকটি ভ্যারিয়েবলের অ্যাড্রেস রাখা হয় সেজন্য ভ্যারিয়েবলের আগে & ব্যবহার করা হয়। & দিয়ে ভ্যারিয়েবলের অ্যাড্রেস পাওয়া যায়। আসুন আমরা একটি সাধারণ প্রোগ্রাম দিয়ে এই অপারেশনস গুলো দেখি।

```c
#include<stdio.h>

int main(void)
{

int a;  // an integer variable

int *ptr; //an integer pointer

a = 10; //assigning a value in the  variable

printf("The value of a is %d", a); //print the value of a
printf("\nThe address of a is %x", &a); //print the address of a. This will print a different value each time

ptr = &a; //assigning the address of a to the pointer

printf("\nAdress stored in ptr is %x", ptr); //printing the address stored in pointer
printf("\nValue of the pointed variable of ptr is %d", *ptr); //accessing the pointed value

a = 76;

printf("\nAdress stored in ptr is (checking again) %x", ptr); //checking the address again, will print the same address
printf("\nValue of the pointed variable of ptr is %d", *ptr); //accessing the new value
printf("\nAddress of the pointer itself is %x", &ptr); //address of the pointer

return 0;
}
```

এখানে আমরা প্রথমে একটি ইন্টিজার `a` নিয়েছি এবং একটি ইন্টিজার পয়েন্টার `ptr` নিয়েছি। এরপরে `a` তে আমরা একটি ভ্যালু অ্যাসাইন করেছি। আমরা প্রথমে `a` এর অ্যাড্রেস ও ভ্যালু প্রিন্ট করেছি। এরপর আমরা `ptr` এ `a` এর অ্যাড্রেস রেখেছি। তারপর `*ptr` দিয়ে আমরা `a` তে রাখা ভ্যালুটিকে অ্যাকসেস করেছি। `a` তে আমরা একটি নতুন ভ্যালু অ্যাসাইন করে আমরা আবার পয়েন্টারের পয়েন্ট করা অ্যাড্রেস ও নতুন ভ্যালু প্রিন্ট করেছি। এখানে লক্ষ্যণীয় পয়েন্টারে রাখা অ্যাড্রেস অর্থাৎ `a` এর অ্যাড্রেস একবারও পাল্টায় নি। আরেকটি বিষয় হল পয়েন্টারগুলো নিজেরাও মেমোরিতে যায়গা নেয় এবং এদেরও অ্যাড্রেস থাকে। একবারে শেষে আমরা `&ptr` দিয়ে আমাদের পয়েন্টারটির অ্যাড্রেসও প্রিন্ট করেছি।
