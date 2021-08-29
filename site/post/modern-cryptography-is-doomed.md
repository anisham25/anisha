---
_archived: false
_draft: false
created-on: "2021-08-24T20:54:43.562Z"
name: "Modern Cryptography is Doomed."
slug: "modern-cryptography-is-doomed"
subheader: "Quantum computing is set to destroy cryptography as we know it"
date: "2019-12-01T00:00:00.000Z"
updated-on: "2021-08-25T02:13:03.862Z"
published-on: "2021-08-25T02:14:02.520Z"
tags: "post"
layout: "single-post.html"
---

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255c65df872b03ef25624d_0*0jGYqaN7ARwg7Jlu.jpeg)

Image Creds: Quanta Magazine

Everything from files on our hard drives to confidential Internet traffic is encrypted by the same system. The system makes up the base of modern cryptography.

**This system is called RSA cryptography.** (It’s doomed, but we’ll get there).

We could talk about the nitty-gritty of the system for a while but the basic point is that it generates keys by **multiplying really big prime numbers**.

It might sound too simple to be true. Our world’s most secure messages are guarded by multiplication?! But it’s actually a really smart idea.

To hack RSA cryptography, you’d have to find the prime factors of the generated keys. While any computer can multiply two really prime numbers, **almost no computer can find the prime factors of that number.** The computer would have to sit there and run through every possibility. They’d never get the job done. (In under a trillion years, that is).

Wait. I said **almost** no computer can break RSA. That’s because a new field of computers is emerging. These computers possess the power to rattle RSA cryptography’s spine.

> **These are quantum computers.**

Quantum computers are weird. They have a bunch of really crazy properties that I talk about [here](https://medium.com/@anishamusti/what-is-quantum-computing-heres-what-you-need-to-know-4f63b95ffeb5). They’re able to perform operations on qubits in superposition which allows them to **reduce the time complexity** of a problem exponentially. What would take a classical computer ²³⁵⁰⁰⁰⁰⁰ steps, it would take a quantum computer **ONE.**

That means that instead of aimlessly searching possibilities to hack RSA, you could get it in **ONE** try.

Yeah, when quantum computers come, RSA’s done for.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255c66434ae0085887d9c1_0*U1e5Vzf7Y2U4D5gB.gif)

RSA on the run

_Let’s break this down more though._

Shor’s Algorithm
----------------

In 1994, a scientist, **Peter Shor**, wrote an algorithm. At this time, the idea of quantum computing was entirely theoretical. Nobody wanted to build one because there was no apparent purpose. This algorithm changed that.

Shor’s algorithm showed that a properly functioning quantum computer could solve problems that classical computers never would. It **kicked off the race** to building a quantum computer.

The algorithm is a 3-part answer to the problem of prime factorization. The first part is performed on a _classical computer_ in polynomial time, but it is only the set-up for the **second and most important part**. The second part requires the use of specially constructed quantum circuits to perform the quantum computation needed to find the value you need for the third part, which allows you to _find the prime factors_ of the integer on a _classical computer_[.](https://interestingengineering.com/how-peter-shors-algorithm-dooms-rsa-encryption-to-failure)¹

It’s a Future Thing.
--------------------

Sadly, **the algorithm is here but the computers aren’t.** Even when Peter Shor came up with it in 1994, he knew it would take an advanced quantum computer to break RSA cryptography.

Luckily (or unluckily), we’re not too far away from developing quantum computers that can break RSA. Most people think that it’ll happen in around a decade.

The best part is that even though RSA cryptography is screwed, we’re not. Cryptographers have already begun research into **Post-Quantum Cryptography** to make sure we’re able to keep everything secure after quantum arrives.

Here’s What I Did.
------------------

I wanted to see Shor’s Algorithm in action. So I made it happen.

There are tons of ways online for people to gain access to quantum simulators and code quantum algorithms. I thought it’d be pretty cool to code Shor’s algorithm and run it on a real simulator at IBM.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255c65e3f9f558af8ec5e6_1*B9kRMMfosTGh4ccydSBexQ.jpeg)

Here’s a snippet of my code

I coded Shor’s algorithm on Qiskit Aqua and ran it on IBM’s simulators. The process wasn’t too bad because there’s a ton of open-source code out there for similar algorithms.

**My results weren’t perfect**. But it’s only a simulator after all. It didn’t always end up working and completely stopped when the numbers got too high.

_But that’s ok._ This is only a glimpse of what a true quantum computer can do. **We’re just hanging on until the real ones show up.**

‍

_My name is Anisha Musti. I’m 14 years old and passionate about quantum computing and artificial intelligence. Thank you for reading and I hope you learned something! Stay up to date for more articles on quantum computing, AI, and other interesting technologies._

Connect with me on LinkedIn [here](https://www.linkedin.com/in/anisha-musti-056703180/) and email me at anisha.musti@gmail.com for any inquiries.
