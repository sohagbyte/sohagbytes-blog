---
title: "সহজ ভাষায় জাভাস্ক্রিপ্ট ভ্যারিয়েবল(Variable)."
seoTitle: "জাভাস্ক্রিপ্ট ভ্যারিয়েবল এর সহজ গাইড।"
seoDescription: "ভ্যারিয়েবল জিনিসটাকে আমরা একটা কন্টেইনার(Container) হিসাবে চিন্তা করতে পারি যেইটাতে আমরা আমাদের ডেটা/ইনফরমেশন গুলো স্টোর করতে পারি।"
datePublished: Mon Jul 15 2024 15:26:46 GMT+0000 (Coordinated Universal Time)
cuid: clyn50vbj00040ame27rubds5
slug: variable-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1721887723778/aa6af46a-f188-45a0-8175-d469657d4514.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1721887740767/37720734-6ea4-4976-afb5-9d46f900cdb9.png
tags: javascript, jsvariable, javascript-variable-in-bangla, variable-in-javascript

---

### ভ্যারিয়েবল কি?

**ভ্যারিয়েবল** জিনিসটাকে আমরা একটা **কন্টেইনার(Container)** হিসাবে চিন্তা করতে পারি যেইটাতে আমরা আমাদের ডেটা/ইনফরমেশন গুলো স্টোর করতে পারি বা সংরক্ষণ করতে পারি এবং যখন দরকার হবে তখন আমরা আমাদের সেই স্টোর করা ডেটাগুলোকে প্রোগ্রামের বিভিন্ন জায়গায় ব্যাবহার করতে পারি।

আমরা যখন কোনো ভ্যারিয়েবল ডিক্লেয়ার করি তখন সেইটা স্টোর হয় আমাদের কম্পিউটারে থাকা মেমোরিতে। অর্থ্যাৎ, মেমোরির কিছু জায়গা বা কিছু স্পেস আমরা রিজার্ভ করে ফেলতেছি একেকটা ভ্যারিয়েবল ডিক্লেয়ার করার মাধ্যমে।

### ভ্যারিয়েবল কেন?

অনেকগুলো কারণে আমরা একটা প্রোগ্রামে ভ্যারিয়েবল ব্যাবহার করে থাকি। তার ভিতরে উল্লেখযোগ্য কিছু কারণ হচ্ছে -

<details data-node-type="hn-details-summary"><summary>ডেটা স্টোরেজঃ</summary><div data-type="detailsContent"></div></details>

একটা প্রোগ্রামে ভ্যারিয়েবল ডিক্লেয়ার করার অন্যতম প্রধান কারণ হচ্ছে ডেটা গুলোকে স্টোর করে রাখা। এমনকি অনেকটা **Structured Way** তে স্টোর করে রাখা, যাতে প্রয়োজন অনুযায়ী আমরা সেইগুলোকে এক্সেস করতে পারি।

<details data-node-type="hn-details-summary"><summary>ডাইনামিক কন্টেন্টঃ</summary><div data-type="detailsContent"></div></details>

ভ্যারিয়েবল এর ব্যাবহার আমাদের প্রোগ্রামকে আরো বেশি ডায়নামিক করে ফেলতে সাহায্য করে। যেমন, কাজের প্রয়োজনে আমাদের অনেক ডেটা চেঞ্জ/মডিফাই করা লাগতে পারে। এই জিনিসটাকে আমরা ভ্যারিয়েবল ব্যাবহার করার মাধ্যমে করে ফেলতে পারি।

<details data-node-type="hn-details-summary"><summary>রিডেবিলিটি বৃদ্ধি করাঃ</summary><div data-type="detailsContent"></div></details>

আমাদের প্রোগ্রামে যখন আমরা সঠিকভাবে ভ্যারিয়েবল এর নামকরন করতে পারি, যেইটা দ্বারা আমাদের ডিক্লেয়ার করা ভ্যারিয়েবল গুলো ঠিক কোন কাজে ব্যাবহার করছি সেইটা বোঝা যায়, তখন সেই প্রোগ্রাম এর রিডেবিলিটি অনেক বেড়ে যায়। পরে যখন অন্য কোনো ডেভেলপার আমাদের লেখা কোডগুলোকে মেইনটেইন করতে যাবে, তখন তারা খুব সহজেই সেই কোডগুলাকে মেইনটেইন করতে পারবে। কারণ তারা অলরেডি জানবে কোন কাজে আমরা কোন ভ্যারিয়েবলটা ডিক্লেয়ার করেছি। এইগুলা ছাড়াও আরো অনেক কারণে, যেমন- একটা প্রোগ্রাম এর **Reusability Increase** করা, **Mathematical/Logical Operation** করা, **Scope Management** করা সহ আমরা আরো অনেক কাজেই আমরা ভ্যারিয়েবল ব্যাবহার করতে পারি।

### ভ্যারিয়েবল নামকরণের নিয়মসমূহঃ

* জাভাস্ক্রিপ্ট হচ্ছে একটা **কেস-সেনসিটিভ(Case-Sensitive)** প্রোগ্রামিং ল্যাঙ্গুয়েজ। এই কেস-সেনসিটিভ কথাটার অর্থ হচ্ছে Capital Letter এ লেখা "A" আর Small Letter এ লেখা "a" দুইটা পুরোপুরি আলাদা জিনিস। এই জিনিসটা মাথায় রেখেই আমাদের ভ্যারিয়েবল ডিক্লেয়ার করা উচিৎ।
    
* ভ্যারিয়েবল এর নামকরনের জন্য আমরা জাভাস্ক্রিপ্টে থাকা রিজার্ভড(Reserved) কিওয়ার্ডস(Keywords) গুলো ব্যাবহার করতে পারব না। যেমন- **if, else, for** ইত্যাদি।
    
* ভ্যারিয়েবল এর নাম অবশ্যই কোনো **Letter, Dollar Sign($)**, বা **Underscore/( \_ )** দিয়ে শুরু করতে হবে।
    
* কোনো ভ্যারিয়েবল এর নাম **Number** দিয়ে শুরু হতে পারবে না, কিন্তু ভ্যারিয়েবল এর নামের শেষে আমরা চাইলে Number ব্যাবহার করতে পারি।
    
* প্রতিটা ভ্যারিয়েবল এর নাম ইউনিক বা একটার চাইতে অন্যটা আলাদা হওয়া দরকার, যাতে একটা থেকে অন্যটাকে সহজেই আলাদা করা যায়। এই ইউনিক নামগুলোকে জাভাস্ক্রিপ্টে **Identifier** ও বলে। এতে করে **Naming Conflict** হয় না।
    
* ভ্যারিয়েবল এর নাম হিসাবে আমরা **Short** **Name** বা **সংক্ষিপ্ত নাম** (যেমনঃ x, y, z) ব্যাবহার করতে পারি আবার **Descriptive** **Name** বা **বর্ণনামূলক** **নাম** (যেমনঃ myName, myAge) ও ব্যাবহার করতে পারি।
    
    আমরা যখন Descriptive Name বা বর্ণনামূলক নাম ব্যাবহার করে ভ্যারিয়েবল ডিক্লেয়ার করব, তখন চাইলে আমরা অনেকগুলো পদ্ধতি অনুসরণ করে সেইটা করতে পারি। যেমন -
    

<details data-node-type="hn-details-summary"><summary>ক্যামেল কেসঃ</summary><div data-type="detailsContent"></div></details>

এই পদ্ধতিতে দুই বা ততোধিক Word কে একসাথে লেখার জন্য প্রথম Word এর প্রথম Letter টা **Small** Letter এ হবে এবং তার পরের সবগুলো Word শুরুর Letter টা **Capital** Letter এ হবে। এই **Camel Case** ই সবচাইতে বেশি ব্যাবহার করা হয়।

**উদাহরণঃ**

```javascript
	let myName = "Sohag";
```

<details data-node-type="hn-details-summary"><summary>স্নেক কেসঃ</summary><div data-type="detailsContent"></div></details>

এই পদ্ধতিতে দুই বা ততোধিক Word কে একসাথে লেখার জন্য বা প্রতিটা নতুন Word কে যুক্ত করার জন্য **Underscore** ব্যাবহার করা হয়।  
  
**উদাহরণঃ**

```javascript
	let my_name = “Sohag”;
```

<details data-node-type="hn-details-summary"><summary>প্যাসকেল কেসঃ</summary><div data-type="detailsContent"></div></details>

এই পদ্ধতিতে দুই বা ততোধিক Word কে একসাথে লেখার জন্য প্রতিটা Word এর **প্রথম Letter** সবসময় **Capital** Letter হবে।  
  
**উদাহরণঃ**

```javascript
	let MyName = "Sohag";
```

উপরের প্রতিটা পদ্ধতিই সঠিক, একেকজন একেকটা পছন্দ করে, এই আরকি!

***স্পেশাল নোটসঃ***

আপনি শুধু যে ভ্যারিয়েবল ডিক্লেয়ার করার জন্যই উপরের পদ্ধতিগুলো অনুসরণ করবেন, এমনটা কিন্তু না। অ্যারে, ফাংশন সহ যেকোনো কিছু ডিক্লেয়ার করার জন্য এই একই নিয়মই প্রযোজ্য হবে।