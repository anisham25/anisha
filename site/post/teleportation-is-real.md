---
_archived: false
_draft: false
created-on: "2021-08-24T20:56:13.403Z"
name: "Teleportation is Real?"
slug: "teleportation-is-real"
subheader: "Yes, and it’s going to change the world"
date: "2020-02-22T00:00:00.000Z"
updated-on: "2021-08-25T02:12:50.515Z"
published-on: "2021-08-25T02:14:02.520Z"
tags: "post"
layout: "single-post.html"
---

For as long as I can remember, I’ve been told teleportation is _fake_. You’ve probably been told the same thing.

When you were a kid and watching Phineas and Ferb build their teleporter, your parents probably told you something along the lines of…

> “Teleportation is a science gimmick.”  
>   
> “It’s just an idea that will never exist.”

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255ca49f5a0c59edf234a8_0*2b-Ef9o01wYLQmGY.jpeg)

Phineas and Ferb’s super cool teleportation device

**But they’re wrong. Everyone who said teleportation is fake, is wrong. Teleportation is real and it’s amazing.**

But, the real teleportation isn’t exactly what we saw in Phineas and Ferb and all our favorite sci-fi movies. It’s not exactly where people are transported from one place to another without ever being in between. It’s a little different.

> The real teleportation is quantum.

In quantum teleportation, we don’t transport _things or people_, we transport _data_.

Imagine if you could share a secret between two people regardless of time, distance, or location.

It would change the world.

How It Works
------------

Let’s use the classic analogy about Alice and Bob.

Alice and Bob are about to travel really far apart. Really far.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255ca47801281228002a00_0*dx3XC2OYibJEQ92L.gif)

But Alice needs a way to send Bob some quantum information while they’re apart. Quantum information is the information of the state of a quantum system.

It can’t be communicated over the phone or in the mail because **if Alice tries to look at her information, she’ll destroy it and Bob will never receive it.** Remember that observing, or measuring, a qubit destroys the superposition of the particle since it is being forced into a set state. I talk a lot about all those details and specifics [here](https://medium.com/@anishamusti/what-is-quantum-computing-heres-what-you-need-to-know-4f63b95ffeb5).

**“So she has to transport it without seeing it. How does she do this?”**

**“Quantum teleportation.”**

To begin, Alice and Bob create a pair of entangled qubits. Think of entanglement like this: you buy a hot dog and a burger. They come in two separate boxes but the second you open Box 1 and see what’s inside, you immediately know what is Box 2. The same goes for entanglement. **Once you measure Qubit 1, you immediately know Qubit 2 is the opposite.**

Both of them take their qubits and head off. **Neither of them looks at their qubits** to prevent destroying it.

Now, Alice needs to teleport her message. All **she needs to do is entangle her message with her qubit** (which is already entangled to Bob’s qubit). When she does this, **Alice’s qubit imprints the state of her message.**

The last step is for Alice to **look at her qubit.** When she looks, both qubits collapse into their respective opposite states.

Bob’s qubit is the opposite of Alice’s but since quantum is strange **he can rearrange the particles** in the opposite way so they’re the exact same.

_That’s quantum teleportation._

I know it sounds crazy. But if you replace Alice’s message with an electron, this is _exactly_ what happens in quantum teleportation.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255ca42219ee454be2a9d1_0*b5T2DJ1FAMTygp2s.gif)

Yes, it is

But there’s one caveat. In order to send Bob the message, Alice had to destroy her own. In quantum mechanics, there is a no-cloning theorem. The theorem states that **it is impossible to make an identical copy of an unknown quantum state.** This prevents us from having clones, or multiple copies of anything we attempted to teleport.

Alice couldn’t just make a copy of her message and send it to Bob. **She had to destroy it** and teleport the instructions for Bob to recreate it.

Now I know it sounds lame. Transporting instructions?! Yeah, I guess it doesn’t sound the same as transporting people. But, there’s more to it than you might think…

The Applications of Quantum Teleportation
-----------------------------------------

As I said before, quantum teleportation doesn’t transport people from one place to another. But, teleportation could also be thought of as transmitting instructions to be rebuilt in another location.

In that sense, **quantum teleportation could be used to teleport people.** We are simply teleporting the information for a human’s molecular makeup so they can be rebuilt elsewhere.

Of course, this won’t happen anytime soon. Keeping particles entangled for a long period of time, over long distances, or along with objects larger than a few atoms is way **beyond what current technology is capable of.** However, with advances in technology, maybe a century from now, our descendants could be teleporting everywhere.

Not only may it be a gateway to real object teleportation, quantum teleportation also has some **practical benefits.**

**Communication would be drastically changed** due to the ensuing secrecy. People would be able to share information at any distance without having to share it with a third-party such as today’s fiber optic cables.

We’re in such early stages that it’s hard to tell just how much quantum teleportation can do for us, but its potential is just waiting to be unlocked.

Personal Project: I Decided To Give Teleportation A Try…
--------------------------------------------------------

Using [Qiskit](https://qiskit.org/), an open source quantum computing software, and simulators at IBM, I attempted to test teleportation on my own. I continued to use the analogy of Alice and Bob for my experiment.

I gave Alice a secret value to represent her message. From there, I coded a series of unitary gates that was applied to the value to combine it with a qubit with ground state, 0.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255ca4e880af3c3435b66d_1*uS8G5mr0xt4c7sFNiZEUMg.png)

The quantum circuit I generated from code

If the circuit works, then the output of the protocol will be the same state passed on to Alice. In the ideal case, and assuming our teleportation protocol works, we will always measure 0 from Bob’s qubit because we started off with 0 from Alice’s.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255ca41728007154dcba10_1*1OkZfRQla6zc-7f8shxETw.png)

The results

Notice that the results on the x-axis in the histogram above are ordered as 𝑐2 𝑐1 𝑐0. We can see that only results where 𝑐2=0 appear, indicating that the teleportation protocol has worked since that is Bob’s qubit.

Unfortunately, the real IBM quantum computers currently do not support instructions after measurements, meaning I could not run the quantum teleportation in its current form on real hardware.

**However, one day, quantum computers, and teleportation, will get there.**

Scientists have already cracked teleportation on the small scale. They’ve teleported information from China to a satellite in orbit. It may only be a matter of time until humans are teleporting, too.

‍

_My name is Anisha Musti. I’m 14 years old and passionate about quantum computing and artificial intelligence. Thank you for reading and I hope you learned something! Stay up to date for more articles on quantum computing, AI, and other interesting technologies._

Connect with me on LinkedIn [here](https://www.linkedin.com/in/anisha-musti-056703180/) and email me at anisha.musti@gmail.com for any inquiries.
