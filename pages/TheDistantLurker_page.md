---
title: The Distant Lurker
date: 2021-12-01
summary: A short game about social engineering and human hacking, made for Game Off 2021.
thumbnail: /images/TheDistantLurker.png?raw=true
badge: Game Off 2021
external_url: https://itch.io/jam/game-off-2021/rate/1282863?=githubio
home_post: true
---

## The Distant Lurker

**Made in under 2 weeks, for Game Off 2021**

- A short game where you social engineer people (NPCs). 
- Hack into the secretive company with a handy kit of tools: 
	- conveniently placed bugs, 
	- email, 
	- and social media
- It comes with _some_ world-building! (if you ignore the plotholes)
- Play the game here: [The Distant Lurker](https://f15hygames.itch.io/the-distant-lurker?=githubio)

---

### Post-mortem Devlog

Note: I've wanted to make a devlog since after the jam but never got around to doing it.
So... better late than never? This is a summarized version because I've got a video version [here](https://youtu.be/HKa_q4zFk2g?si=Dyo_xwpHVlaDsmq2).

Anyway, it did surprisingly well! Out of 502 entries, it got #55 overall, and #25 in innovation :D
(It's been 4 years and it's still my most significant project)


**The Premise**

I just finished national exams and was itching to get back into game dev, so I decided to join Game Off 2021.
The gimmick was that we had to use Github to publish our source code. 
It was my first time properly using Github, and I didn't get the appeal of it (foreshadowing).

The theme was "Bug", and after some ideation, I went for this definition:
> Conceal a miniature microphone in (a room or device) in order to listen to or record someone's conversations secretly.

I was learning a lot about cybersecurity and participating in capture the flags during this period, which was why I decided to make this game about hacking.
I didn't have enough knowledge to get into anything technical, which was why I stuck with the educational message of human hacking.


**The Process**

Through the 2 weeks, I watched a bunch of tutorials and cobbled together an OS based system, with 3 "hacking tools".

1. **Bug:** You can listen in on office worker's conversations to glean their personal information.
<img src="../images/TDL_Bug.jpg?raw=true"/>

2. **Email:** Using anyone's full name and password, you can access their email inbox.
<img src="../images/TDL_Email.jpg?raw=true"/>

3. **Instasnap:** You can search up anyone's full name to find their social media posts.
<img src="../images/TDL_Instasnap.jpg?raw=true"/>


I made up a small company and made up interconnected stories and dynamics for each worker to create their accounts.

I considered creating voice overs of the bug's dialogues but I knew I couldn't create 3-4 different voices. 
...which was why I resorted to using one of those sketchy AI voice websites. 
(Back in the day,) I couldn't find any good sounding AI voices without forking up a fee. 
So I chose to incorporate the AI sounding voices as part of the storyline :)

(It's a feature, not a bug)

I also had a lot of fun drawing everyone's "social media posts" and creating backstories for side characters.

Things were going well... until it didn't.


**The Problem**

The first problem that arose was that the audio visualiser refused to work on the web build. 
Even after much googling and debugging, I couldn't get it to work. So I scrapped it for a subtitling feature instead.
This might have been a blessing in disguise because in hindsight, it would have been very difficult for people to decipher some of the key information, like complicated passwords.

The second problem, the project corrupted and started creating a bunch of engine-related errors.
No matter how much I restarted the engine and my system, it stuck around.

So thank goodness for needing to use Github in this jam. I only had to redo a day's worth of work, 
instead of 1.5 weeks worth. Definitely taught me a great lesson on version control.

**Conclusion**

So yea. I forgot what else I intended to say. The results turned out surprisingly well. 

<img src="../images/TDL_results.png?raw=true"/>

**Post conclusion**

I developed the game a little more this year (2025) for a uni module. Video of gameplay [here](https://www.youtube.com/watch?v=kgsAbbHFfvo)
- I added some commonly asked for functionality. (copy-paste)
- Made tabs actually work like tabs. (draggable, overlappable, closeable)
- Added some optional content (notepad tips)

<img src="../images/TheDistantLurker.png?raw=true"/>

I'd be interested in making a second game with a new story, but unfortunately I haven't had many good ideas.

So... maybe someday? 

Or if anyone has any suggestions?



<p>
<a href="{{ "/" | relative_url }}">← Back to Home</a>
</p>