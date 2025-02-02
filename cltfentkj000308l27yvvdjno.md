---
title: "Scope in JavaScript"
seoTitle: "Scope in Javascript in bangla"
seoDescription: "Scope এর মাধ্যমে আমরা জানতে পারি যে, আমাদের Declare করা Variable বা function গুলো আমরা একটা প্রোগ্রামের কোন কোন জায়গায় Access করতে পারি।"
datePublished: Wed Mar 06 2024 06:15:52 GMT+0000 (Coordinated Universal Time)
cuid: cltfentkj000308l27yvvdjno
slug: scope-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1709716688526/bbe6dbaf-5322-4fbe-977e-0fe1ac9a1bdc.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1709716757782/15c9f6b7-d5c4-4855-bce7-44dfa14b0628.png
tags: scope-in-js, js-scope, scope-in-javascript, javascript-scope-in-bangla, javascript-bangla

---

## What is Scope:

**Scope** জাভাস্ক্রিপ্টে খুবই গুরুত্বপূর্ন একটা Concept. **Scope** এর মাধ্যমে আমরা জানতে পারি যে, আমাদের Declare করা Variable বা function গুলো আমরা একটা প্রোগ্রামের কোন কোন জায়গায় Access করতে পারি।

**Note-1:** জাভাস্ক্রিপ্টে **Object** এবং **Function** ও কিন্তু Variable.

## Types of Scope:

জাভাস্ক্রিপ্টে সাধারণত ৩ ধরনের Scope আছে-

1. **Block Scope.**
    
2. **Function Scope.**
    
3. **Global Scope.**
    

### **Block Scope:**

জাভাস্ক্রিপ্ট এর **<mark>ES6</mark>** Version আসার আগে পর্যন্ত Variable এর শুধুমাত্র ২ টা Scope ছিলো-

1. **Function Scope.**
    
2. **Global Scope.**
    

কিন্তু জাভাস্ক্রিপ্ট **<mark>ES6</mark>** Version এ ২০১৫ সালে আরো নতুন ২ টা **Keyword** Introduce করানো হয়, যার একটা হচ্ছে `let` এবং অপরটা হচ্ছে `const`. এই ২ টা Keyword এর সাথে জাভাস্ক্রিপ্টে আরো নতুন একটা **Scope** যোগ করে যেইটা হচ্ছে **<mark>Block Scope.</mark>** অর্থ্যাৎ, জাভাস্ক্রিপ্ট এর **<mark>ES6</mark>** Version এ `let` এবং `const` - এই ২টা Keyword এর সাথে **BlockScope** ও নতুন **Scope** হিসাবে যোগ হয়।

**Note-2:**`var` এবং `let` ব্যাবহার করা হয় **Variable** Declare করার জন্য, এবং `const` ব্যাবহার করা হয় **Constant** Declare করার জন্য।

**Note-3:**`var` হচ্ছে **<mark>Global</mark>** Scoped Variable এবং একইসাথে **<mark>Function</mark>** Scoped Variable. আর `let` এবং `const` হচ্ছে **<mark>Block</mark>** Scoped variable.

কিন্তু **Block Scope** জিনিসটা আসলে কি ? বা আমরা কিভাবে বুঝতে পারব যে, এইটা Block Scoped কি না?

Block Scope বোঝার জন্য প্রথমে আমাদের Block জিনিসটা কি সেইটা আগে জানা দরকার। **Block** বলতে এইখানে দুইটা **<mark>Curly Bracket / {}</mark>** কে বোঝানো হচ্ছে। অর্থ্যাৎ, এই ২টা Curly Bracket এর ভিতরে যেই কোড গুলো থাকবে সেইগুলাই Block Scoped, বা এর ভিতরে যেই Variable গুলো থাকবে সেইগুলাই **<mark>Block Scoped</mark>** Variable.

`let` এবং `const` হচ্ছে Block Scoped Variable, অর্থ্যাৎ, আমরা যখন কোনো Block এর ভিতরে `let` এবং `const` ব্যাবহার করে কোনো Variable Declare করবো, তখন সেইটা সেই Block এর বাইরে থেকে **Access** করতে পারব না। এইটা বোঝার জন্য নিচের উদাহরন টা খেয়াল করেন -

**Example using <mark>let</mark> keyword:**

```javascript
{
    let age = 20;
}
console.log(age);
//ReferenceError: age is not defined.
```

উপরের প্রোগ্রামটা Run করলে আমরা একটা **<mark>Reference Error</mark>** পাবো, যেইটা আমাদের কে বলছে যে, `age` নামের কোনো Variable **Define** ই করা হয় নি। কারণ আমরা জানি, `let` ব্যাবহার করে কোনো Block এর Variable Declare করলে Block এর বাইরে আমরা সেই Variable টা Access করতে পারি না। তাই আমরা উপরের Error টা পেয়েছি।

**Example using <mark>const</mark> keyword:**

```javascript
{
    const age = 20;
}
console.log(age);
//ReferenceError: age is not defined
```

এইবার উপরে আমরা `const` ব্যাবহার করে একটা Block এ Variable Declare করেছি, কিন্তু আমরা জানি, `let` এর মত `const` ও হচ্ছে Block Scoped Variable, তাই এইখানেও একই ধরনের Error পাবো, যেমনটা উপরে আমরা `let` এর ক্ষেত্রে পেয়েছিলাম।

**Example using <mark>var</mark> keyword:**

```javascript
{
    var age = 20;
}
console.log(age);
//20
```

উপরে আমরা একটা Block এর ভিতরে var ব্যাবহার করে Variable Declare করেছি, কিন্তু এইখানে একটা মজার ব্যাপার খেয়াল করেছেন? এইখানে কিন্তু আমরা ঠিকঠাক Result ই পাচ্ছি। কিন্তু কেন? এইটার কারণ হলো var হচ্ছে Global Scoped Variable. যার কারণে আমরা Block Scope এর বাইরে থেকেও এর Access পাচ্ছি। ঠিক এই কারণেই var ব্যাবহার না করার জন্য অনেকে Recommend করে থাকে। কারণ এতে Naming Conflicts হওয়ার সম্ভাবনা থাকে। var নিয়ে আরেকটা Twist আছে, যেইটা আমি Function Scope এ আলোচনা করেছি।

উপরে আমরা Block জিনিসটা যেইভাবে ব্যাবহার করেছি, একটা প্রোগ্রামে ঠিক সেইভাবে আসলে আমরা একটা Block ব্যাবহার করি না। শুধুমাত্র, বোঝানোর সুবিধার্তে এইরকম ভাবে **Block** ব্যাবহার করেছি।

এই Block গুলো কিন্তু আমরা অনেক জায়গায় ব্যাবহার করি বা দেখি, যেমন- কোনো ফাংশনে, লুপে, কন্ডিশনাল স্টেটমেন্টে, অবজেক্টে ইত্যাদি ইত্যাদি। নিচে কয়েকটার উদাহরণ দেখা যাক -

```javascript
//Block in Function
function girlFriend() {
    let gf = 'Purnima';
    console.log(gf);
};

//Block in for loop
for (let i = 0; i <= 5; i++) {
    console.log('Purnima');
};

//Block in Conditional Statement
let gf = 'Purnima'
if (gf == 'Purnima') {
    console.log(`That's my Girlfriend`);
};
```

### **Function Scope:**