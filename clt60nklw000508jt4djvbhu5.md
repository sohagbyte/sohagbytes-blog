---
title: "Intro to javaScript Variable - Bangla"
seoTitle: "Javascript Variable in Bangla"
seoDescription: "Variable জিনিসটাকে আমরা একটা Container হিসাবে চিন্তা করতে পারি যেইটাতে আমরা আমাদের Data/Information গুলো Store/সংরক্ষণ করতে পারি এবং যখন দরকার হবে ......"
datePublished: Wed Feb 28 2024 16:33:50 GMT+0000 (Coordinated Universal Time)
cuid: clt60nklw000508jt4djvbhu5
slug: intro-to-javascript-variable-bangla
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1709137959429/6143d23e-919f-4458-b97a-458a24c4fd14.png
tags: javascript, jsvariable, javascript-in-bangla, javascript-variable-in-bangla

---

### **What is Variable?**

Variable জিনিসটাকে আমরা একটা Container হিসাবে চিন্তা করতে পারি যেইটাতে আমরা আমাদের Data/Information গুলো Store/সংরক্ষণ করতে পারি এবং যখন দরকার হবে তখন আমরা আমাদের সেই Store করা Data গুলোকে প্রোগ্রামের বিভিন্ন জায়গায় ব্যাবহার করতে পারি, বা সেইগুলোকে নিয়ে কাজ করতে পারি।

আমরা যখন কোনো Variable Declare করি তখন সেইটা Store হয় আমাদের কম্পিউটারে থাকা Memory তে । অর্থ্যাৎ, মেমোরির কিছু জায়গা/Space **Reserve** হয়ে যাচ্ছে একেকটা Variable Declare করার মাধ্যমে।

### **Why Variable?**

অনেকগুলো কারণে একটা Program এ আমরা Variable ব্যবহার করে থাকি। তার ভিতরে উল্লেখযোগ্য কিছু কারণ হচ্ছে -

<details data-node-type="hn-details-summary"><summary>Data Storage:</summary><div data-type="detailsContent">একটা Program এ Variable ব্যাবহার করার অন্যতম প্রধাণ কারণ হচ্ছে Data গুলোকে Store করে রাখা। এমনকি অনেকটা Structured way তে Store করে রাখা, যাতে প্রয়োজন অনুযায়ী আমরা সেইগুলোকে Access করতে পারি।</div></details><details data-node-type="hn-details-summary"><summary>Dynamic Content:</summary><div data-type="detailsContent">Variable এর ব্যাবহার আমাদের Program কে আরো বেশি Dynamic করে ফেলতে সাহায্য করে। যেমন কাজের প্রয়োজনে আমাদের অনেক Data Change/Modify করা লাগতে পারে। এই জিনিসটা আমরা Variable ব্যাবহার করার মাধ্যমে করে ফেলতে পারি।</div></details><details data-node-type="hn-details-summary"><summary>Increase Readability:</summary><div data-type="detailsContent">আমাদের Program এ যখন সঠিক Variable এর নামকরণ করতে পারি যেইটা দ্বারা আমাদের Declare করা Variable টা ঠিক কি কাজ করছে সেইটা বোঝা যায়, তখন সেই Program তার <strong>Readability</strong> অনেক বেড়ে যায়। পরে যখন অন্য কোনো ডেভেলপার আমাদের লেখা কোডগুলোকে <strong>Maintain</strong> করবে তখন তারা খুব সহজেই সেইগুলাকে Maintain করতে পারবে। কারণ তারা Already জানবে ঠিক কোন কাজে আমরা কোন Variable টা Declare করেছি।</div></details>

এইগুলা ছাড়াও আরো অনেক কারণে যেমন একটা Program এর **Reusablity Increase** করা, **Mathematical/Logical Operations** করা, **Scope Management** করা সহ আরো অনেক কাজেই আমরা Variable ব্যাবহার করতে পারি।

### **Variable Naming Rules in JavaScript:**

* জাভাস্ক্রিপ্ট হচ্ছে একটা **Case Sensitive** প্রোগ্রামিং Language. যেইটার অর্থ হচ্ছে **Capital Letter** এ লেখা **“A”** আর **Small Letter** এ লেখা **“a”** দুইটা পুরোপুরি আলাদা জিনিস। এই জিনিসটা মাথায় রেখেই আমাদের Variable এর নামকরণ করা উচিৎ।
    
* Variable এর নামকরণের জন্য আমরা জাভাস্ক্রিপ্টে থাকা **Reserved Keywords** গুলো ব্যাবহার করতে পারব না।
    
* Variable এর নাম অবশ্যই কোনো **Letter, Dollar sign($),** বা **Underscore(\_)** দিয়ে শুরু করতে হবে।
    
* কোনো Variable এর নাম Number দিয়ে শুরু হইতে পারবে না, কিন্তু নামের শেষে আমরা চাইলে Number ব্যাবহার করতে পারি।
    
* প্রতিটা Variable এর নাম **Unique** বা একটার চাইতে অন্যটা আলাদা হওয়া দরকার, যাতে একটা থেকে অন্যটাকে সহজেই আলাদা করা যায়। এই ইউনিক নামগুলাকে জাভাস্ক্রিপ্টে Identifier ও বলে। এতে করে Naming Conflict হয় না।
    
* Variable এর নাম হিসাবে আমরা **Short Name** (x, y, i etc etc) ও ব্যাবহার করতে পারি, আবার **Descriptive Name** (myName, Number1 etc etc) ও ব্যাবহার করতে পারি।
    

আমরা যখন **Descriptive Name/বর্ণনামূলক নাম** ব্যাবহার করে Variable Declare করি তখন চাইলে আমরা অনেকগুলো Method Follow করে সেইটা করতে পারি। যেমন -

<details data-node-type="hn-details-summary"><summary>Camel Case:</summary><div data-type="detailsContent">এই পদ্ধতিতে দুই বা ততোধিক Word কে একসাথে লেখার জন্য প্রথম Word এর প্রথম Letter টা Small Letter এ হবে এবং তার পরের সবগুলো Word শুরুর Letter টা Capital Letter এ হবে। এই Camel Case ই সবচাইতে বেশি ব্যাবহার করা হয়।</div></details>

***Example***:

```javascript
let myName = “Sohag”;
```

<details data-node-type="hn-details-summary"><summary>Snake Case:</summary><div data-type="detailsContent">এই পদ্ধতিতে দুই বা ততোধিক Word কে একসাথে লেখার জন্য বা প্রতিটা নতুন Word কে যুক্ত করার জন্য Underscore(_) ব্যাবহার করা হয়।</div></details>

***Example:***

```javascript
let my_name = “Sohag”;
```

<details data-node-type="hn-details-summary"><summary>Pascal Case:</summary><div data-type="detailsContent">এই পদ্ধতিতে দুই বা ততোধিক Word কে একসাথে লেখার জন্য প্রতিটা Word এর প্রথম Letter সবসময় Capital Letter হবে।</div></details>

***Example:***

```javascript
let MyName = “Sohag”;
```

উপরের প্রতিটা পদ্ধতিই সঠিক, একেকজন একেকটা Prefer করে, এই আরকি!

**<mark>Special Note:</mark>**

আপনি শুধু যে Variable Declare করার জন্য উপরোক্ত Method গুলো Follow করবেন, এমনটা কিন্তু না, Array, Function সহ যেকোনো কিছু Declare করার জন্য এই একই নিয়মই প্রযোজ্য হবে।