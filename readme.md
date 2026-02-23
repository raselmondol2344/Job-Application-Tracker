## Answers 

### 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

*** getElementById() : নির্দিষ্ট id দিয়ে element ধরে
*** etElementsByClassName () :  নির্দিষ্ট class দিয়ে element ধরে
*** querySelector() : CSS selector দিয়ে   প্রথম element  ধরে 
*** querySelectorAll() :  CSS selector দিয়ে সবগুলো element  ধরে

### 2. How do you create and insert a new element into the DOM?
*** নতুন element বানাতে document.createElement() দিয়ে আগে element তৈরি করি, তারপর তার ভিতরে লেখা বসাই। এরপর append() বা appendChild() দিয়ে সেটাকে parent element এর ভিতরে ঢুকিয়ে দিলে সেটা DOM এ দেখা যায়।
### 3. What is Event Bubbling? And how does it work?
*** event প্রথমে যে element এ ঘটে সেখানে কাজ করে, তারপর ক্রমান্বয়ে উপরের element গুলোতেও পৌঁছে যায়।

### 4. What is Event Delegation in JavaScript? Why is it useful?
Event Delegation হলো JavaScript-এর একটি কৌশল যেখানে একাধিক child element-এ আলাদা আলাদা event listener না দিয়ে তাদের parent element-এ একটি event listener যোগ করা হয়, এবং event bubbling ব্যবহার করে নির্দিষ্ট target element শনাক্ত করা হয়।

### 5. What is the difference between preventDefault() and stopPropagation() methods?
*** preventDefault() ব্যবহার করলে কোনো element-এর নিজস্ব ডিফল্ট কাজ বন্ধ হয়ে যায়, আর stopPropagation() ব্যবহার করলে event তার parent element-এ আর ছড়িয়ে যেতে পারে না।