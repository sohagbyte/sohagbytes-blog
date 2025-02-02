---
title: "Comment in JavaScript - Bangla"
seoTitle: "Javascript comment in bangla"
seoDescription: "Comment মূলত জাভাস্ক্রিপ্ট কোড গুলোকে আরো অনেক বেশি Readable করতে সাহায্যে করে।"
datePublished: Tue Feb 27 2024 05:50:59 GMT+0000 (Coordinated Universal Time)
cuid: clt3y9000000108jshxpza1id
slug: comment-in-javascript-bangla
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1709030155233/03df8e03-181d-4e94-bde2-52c771707513.png
tags: javascript, javascript-comments, javascript-in-bangla, sinle-line-comment-in-js, multi-line-comment-in-js

---

### **JavaScript Comment:**

জাভাস্ক্রিপ্টে <mark>Comment</mark> অন্যতম গুরুত্বপূর্ণ একটা বিষয়। আমরা যখন একসাথে অনেক কোড লিখি, তখন অন্য ডেভেলপার হয়ত আমাদের কোড দেখে বুঝতে নাও পারে যে, আমরা আসলে কোন প্রয়োজনে কোড গুলো লিখেছি। কিন্তু আমরা যদি কোডে <mark>Comment</mark> করে রাখি, তাহলে অন্য ডেভেলপার খুব সহজেই বুঝতে  পারবে আমরা কোন প্রয়োজনে কোন কোড গুলো লিখছি।

এক কথায় বলতে  গেলে, Comment মূলত জাভাস্ক্রিপ্ট কোড গুলোকে আরো অনেক বেশি <mark>Readable</mark> করতে সাহায্যে করে।

আরেকটা গুরুত্বপূর্ণ কথা হচ্ছে, এই Comment গুলোকে কিন্তু জাভাস্ক্রিপ্ট  <mark>Execute</mark> করে না, জাস্ট <mark>Ignore </mark> করে চলে যায় (Like my Crush!😞)

### **Types of Comment:**

**জাভাস্ক্রিপ্টে মূলত ২ ধরনের Comment আছে-**

*১. সিঙ্গেল লাইন কমেন্ট (Single Line Comment)*

*২. মাল্টি লাইন কমেন্ট (Multi Line Comment)*

#### **Single Line Comment:**

এক লাইন বা Single Line জন্য মূলত Single Line Comment ব্যাবহার করা হয়। আপনি চাইলে একের অধিক লাইনের Comment এর জন্য ও Single Line Comment ব্যাবহার করতে পারেন। Single Line Comment শুরু হয় দুইটা <mark>Forward Slash (//)</mark> দিয়ে । এই ২ টা Forward Slash এর পরে যা থাকবে সেটুকুই Comment আকারে থাকবে।

**উদাহরনঃ**

```javascript
//It will print Hello World! in console.
console.log('Hello World!');
```

#### **Multi Line Comment:**

উপরে আমরা দেখেছি Single Line Comment যা মূলত Multi Line Comment এর ক্ষেত্রেও আপনি চাইলে ব্যাবহার করতে পারবেন, কিন্তু আসলে <mark>Recommended</mark> হচ্ছে Single Line এর জন্য Single Line Comment এবং Multi Line এর জন্য Multi Line Comment ব্যাবহার করা।

মাল্টি লাইন কমেন্ট শুরু হয় **<mark>*/</mark>** দিয়ে এবং মাঝখানে থাকবে যে অংশটুকু কমেন্ট করতে চাচ্ছি সেইটুকু এবং কমেন্ট শেষ হবে **<mark>*/</mark>** দিয়ে।

**উদাহরনঃ**

```javascript
/*
This function is for doing sum of two 
numbers. It will not execute.
*/
function sum(num1, num2) {
    console.log(num1 + num2);
}
sum(20, 25);
```