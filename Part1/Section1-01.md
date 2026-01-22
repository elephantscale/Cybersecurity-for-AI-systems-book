# Introduction to AI Security
* In this introduction, we cover a few important questions
  * How this book came to be
  * What is it based on
  * What is in it for you, the reader

### How this book came to be
This book started as a request from a large multinational company for
"AI and Cybersecurity" course. However, and you may have the same question -
Who needs whom? Will AI enhance your cybersecurity posture? 
That falls under the purview of security companies, even though 
a software developer with an interest in AI might benefit from it.

Or, should AI benefit from Cybersecurity? That would mean that someone has already built
A large collection of AI applications is looking to protect them from hackers.

In any case, I offered the course for another large client of mine and immediately 18 
engineers signed up. But then I was in for a surprise. Even though the course was titled
"How to protect the AI systems you have built", very few of my students had actually
built something.

This is how I understood that the book should be about everything:
  * How to build AI applications
  * How to protect them once you have built them
  * How can AI help cybersecurity?

Accordingly, this book includes all three. First, I outline basically what you build,
be it AI that helps you order a pizza, talk to your documents, or make your database
answer questions based on your data. You may even be looking for a way to productize the AI system
that you have built and scale it up. In any case, you want it to be secure.
 
Secondly, I will demonstrate how hackers can exploit what you have built.
Thirdly, I will show you what the best practices protecting your systems are, and
why you should not rely on your home-grown ideas, but keep reading this book.

### An important note on creating your own AI apps

You will not have to do it! Having read that my students in class did not have applications to protect,
you might feel intimidated and think, "Am I the same?" No such thing! I have prepared these applications for you.
The accompanying GitHub repository, <TODO insert the link>, has everything you need. This repository contains Terraform scripts
that will build the AI applications you need. GitHub is ideally suited for that. 

You will use the mechanism provided by GitHub called "Actions." So, you will use the scripts that I provide.
Run them within GitHub, and have a ready-to-run AI application. Then you can attack them.

I will also provide a brief overview of the AI architecture I use. The added benefit of this approach is that you
will get a concise introduction to various ways of building AI apps. Here, I have to acknowledge the inspiration from 
AIGoat Labs (https://github.com/elephantscale/AIGoat.) by Ofir Yakobi and Shir Sadon.

### What is the book based on

This book is based on my long-standing interest in Cybersecurity. I infected my son with it, and
he became a cybersecurity consultant. I follow Cybersecurity figures such as Jeremiah Grossman,
the founder of WhiteHat Security, and Grugq, the “most quoted man in infosec".

For the past three years, I have been hosting a weekly webinar titled "Advances in AI." There, I would review the latest 
technologies that anyone interested in building AI applications can use.

I have delivered multiple Cybersecurity training sessions to developers at Fortune 200 companies and government agencies.
It is this teaching that proved most useful. As an ancient philosopher said, 
"I have learned a lot from my teacher, more from my colleagues, but most from my students."

In teaching these classes, and especially those that were advertised in my client's company using the
"open enrollment" system, I saw an interesting phenomenon. Many students would sign up for the course because
"it sounded cool." However, when I suggested, as an exercise, that the students start working on protecting AI applications that the students had built,
the majority did not have anything to protect. They have not built any! Thus, I learned that I need to
teach how to build an AI application first, and then grow to defend it. This experience has led to a
book plan that I am describing below.

### What is in this book for you
* The book explains, as briefly as possible but still in sufficient detail, how you would build a specific AI application.
This may involve AI interacting with your documents, accessing your data in a database, or providing the user with advice.
Not every person in the world is an AI Gen Engineer, at least not yet. Having built an AI app, the reader is
ready to enumerate the ways it can be attacked (Threat Modeling) and then proceed to building defenses. 
* This approach makes sure that the reader is not bored and that the reader and the writer are on the same page
about the application that we will build and then protect.
* In a class, I would follow a 50% lecture, 50% lab rule. In this book, I give enough exercises and challenges 
to convert theory into practice.
* Any reader will appreciate the cops-and-robbers game that is implicit in hacking. In addition,
I will make the reading pleasant. In the words of the immortal author of "The Golden Ass",
"Whereunto gentle Reader, if thou wilt give attendant eare, it will minister unto thee
such delectable matter as thou shalt be contented withall." In short: reader, enjoy!

### A vital principle: do not say obvious things
* As one university professor once taught me: if you can Google it, I do not have to teach you that.
That is, if you can find the information yourself, it is worthless to put it in the book.
What makes this book really useful is that you CANNOT find these texts elsewhere. 
* Incidentally, that is also good advice if you are looking to detect pieces written by AI.

  ### Tips
  As you go through the book, you will occasionally encounter tips or actionable recommendations. I will mark it as such, **Tip!**
  So, the first tip: in cybersecurity, taught by a wise person, even mundane everyday matters are essential, and you can learn from them.

