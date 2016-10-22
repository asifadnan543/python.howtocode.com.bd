## কোডের পুনব্যবহার  

কম্পিউটারের জন্য প্রোগ্রাম বা ইন্সট্রাকশন লিখে আমরা কম্পিউটারকে দিয়ে একটি কাজ বার বার করিয়ে নিতে পারি। এটুকু আমরা সবাই জানি। একটি কাজের জন্য এক একজন এক একভাবে প্রোগ্রাম লিখতে পারে। যেমন আমাদের যদি স্ক্রিনে ১০টি লাইন প্রিন্ট করতে হয় তখন কেউ হয়তো একটি প্রোগ্রাম লিখে তার মধ্যে ১০টি প্রিন্ট স্টেটমেন্ট ব্যবহার করবে। আবার ভালো প্রোগ্রামাররা এই কাজের জন্য লুপ ব্যবহার করবে। আগের চ্যাপ্টারেই আমরা `for`, `while` ইত্যাদি লুপের ব্যবহার দেখেছি। লুপ ব্যবহার করে এর মধ্যেকার নির্দিষ্ট কিছু ইন্সট্রাকশনকে একাধিকবার এক্সিকিউট করানো যায়। এটা এক ধরণের কোডের পুনব্যবহার। অর্থাৎ ১০ বার প্রিন্ট স্টেটমেন্ট ব্যবহার না করে একটি প্রিন্ট স্টেটমেন্ট এবং সাথে একটু লজিক ব্যবহার করে একই কাজ করা সম্ভব।   

যেকোনো রকম কম্পিউটার প্রোগ্রামিং -এ দুটি টার্ম শুনতে পাওয়া যায়। **WET** এবং **DRY**. WET মানে বলা হয় **Write Everything Twice** অথবা **We Enjoy Writing**. অর্থাৎ যেকোনো প্রোগ্রামের মধ্যে অপ্রয়োজনীয় এবং অতিরিক্ত স্টেটমেন্ট লেখা বা ব্যবহার করা যেখানে সেই একই কাজ অনেক কম কোড লিখেও আরও অপ্টিমাইজ ভাবে করা যেত। এটা খারাপ অভ্যাস। আবার DRY মানে বলা হয় - **Do not Repeat Yourself**. অর্থাৎ ওই যে ১০ বার ১০টা লাইন প্রিন্ট করার জন্য ১০ বার প্রিন্ট স্টেটমেন্ট ব্যবহার না করা। যেহেতু কাজটা একই (কিছু একটা প্রিন্ট করা) সেহেতু একবার প্রিন্ট স্টেটমেন্ট লিখেই কোন না কোন ভাবে ১০ বার প্রিন্ট করা সম্ভব। এটা ভালো অভ্যাস।  

এরকম কোড পুনব্যবহার করার সবচেয়ে ভালো উদাহরণ হচ্ছে ফাংশন এর প্রয়োগ। আমরা কিন্তু ইতোমধ্যে ফাংশনের ব্যবহার করে ফেলেছি আগের চ্যাপ্টার গুলোতে। যেমন এই যে প্রিন্ট `print` নিয়ে এতো কথা বলা হল, এটাও একটা ফাংশন। এটা একটা বিল্ট ইন ফাংশন। অর্থাৎ এই ফাংশনের কর্মপ্রণালী আমরা নিজেরা কোড করে লিখি নাই। এই ফাংশনের কাজ হচ্ছে - এর মধ্যে যেকোনো string কে পাঠিয়ে দিলে সেই string -কে সে স্ট্যান্ডার্ড আউটপুটে প্রিন্ট করে দেখায়। অর্থাৎ, কোন কিছু প্রিন্ট করার জন্য আমরা প্রত্যেকবার কম্পিউটারের বোধগম্য এক গাদা কোড লিখি না। শুধু প্রিন্ট ফাংশনকে কল করে যা প্রিন্ট করতে হবে তা ওকে দিয়ে দেই। এভাবে আমরা প্রিন্ট ফাংশনের জন্য করা কোডকে বার বার ব্যবহার করছি। এটাই কোডের পুনব্যবহার।   

সামনের কয়েকটি চ্যাপ্টারে আমরা নিজেদের বিভিন্ন কাজের জন্য ফাংশন লিখে কোডের পুনব্যবহার দেখবো।   