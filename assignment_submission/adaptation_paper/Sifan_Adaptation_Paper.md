# Case Study: The Adaptation of HUST Online Judge
#### Instructor: James Howison
#### Student: Sifan Guo

## 1 Introduction
### 1.1 People Who Started This Project
About 10 years ago in 2008, _Sempr_, a former member of Huazhong University of Science and Technology(  [HUST](https://en.wikipedia.org/wiki/Huazhong_University_of_Science_and_Technology)) [ACMICPC](https://en.wikipedia.org/wiki/ACM_International_Collegiate_Programming_Contest) team, had an idea of building an online judge[1] both for their team's algorithm training and for his own graduation project. Although many successful projects are created by a single person, more people are needed in order to perfect them. According to one former participant Shang(my interviewee), before _Sempr_ began coding, he discussed this idea with his teammates and their team's advisors, undoubtedly, they all encouraged him to fulfill it and they promised to offer help when needed. Through the efforts of all these people, the HUST Online Judge first came out with the domain acm.hust.edu.cn which was no longer used after Jan 2018 due to many reasons.


### 1.2 Embracing the Wonderful GPL v2 License!
It was no later than a week after HUSTOJ started its service when the team decided to share their codes on [Google Code](https://code.google.com/archive/p/hustoj/) under the GNU General Public License, version 2. Shang told me that their team made this decision for many reasons:

1. Their teammates were all busy training and the fact that they were good at algorithms doesn't necessarily mean they were capable of programming. They all agreed that they could turn to more people for help.

2. The online judge was good enough for them, and they want more users to join and offer feedbacks because more people would have more different viewpoints which could help them to improve the online judge in various ways.

3. Most contributors of this project were senior students, and they were afraid of being too busy to contribute after the graduation.

4. As mentioned in the second reason, they thought highly of their online judge, so they wanted to share their codes with the world and "show off".

5. The staff of HUST considered it as a great way to expand the influence of the university, also, this can be counted as their working achievements.


### 1.3 Becoming Popular
As more and more universities began to have teams for ACMICPC, they attached great significance to building their own online judge system because they can customize the system and flexibly host their own competitions. Including many high schools, 126 organizations (most of them are universities: [check the whole list here](https://code.google.com/archive/p/hustoj/)) throughout the world had used the HUST Online Judge or designed their own system based on it. According to Shang, HUST Online Judge was well-known to domestic ACMICPC teams then. In a word, it was definitely a successful project around 2010.


### 1.4 Without the Domain hust.edu.cn, What Would HUST Online Judge Be?
After Jan 2018, the origin domain acm.hust.edu.cn was no longer used after nearly 10 years of service. There are two websites -- [hustoj.org](http://www.hustoj.org) and [hustoj.com](http://www.hustoj.com/), both of them claimed to be HUST Online Judge but neither provides the real judging service as acm.hust.edu.cn used to. The hustoj.org offers English version and works as a backup which retains the original data but submission hasn't been enabled yet. On the other hand, hustoj.com does provide demo submission and judge service, however, unlike non-profit service, it seems to be a commercial website which is selling the customer service[2].

I asked Shang why the domain was changed and he indicated that it's the university's decision. In addition, he said we can't know the real reasons which made the university decide not to offer her domain and servers anymore. I tried to contact the staff but no one responded, as a result, what I'm going to say are all based on my conjecture, **please don't hesitate to let me know by pulling request or adding issues, if anyone has the other stories of HUST Online Judge. I'll be more than happy to update this paper in no time.**

After in-depth discussion with Shang, we both agreed the commercialization of HUST Online Judge would be direct cause. In most Chinese universities, they are only allowed to offer online services or other alike resources to their students for academic use only, otherwise things would become too complicated because applying for commercial projects requires approval of many departments of the university. In other words, if we're making money by using resources of the organization without supervision, it's like cheating. Case in point, an active contributor of HUST Online Judge and also the administrator of hustoj.com _zhblue_ is selling his service. Although _zhblue_ is not from HUST, he did play an irreplaceable role in promoting HUST Online Judge by offering paid service. Because even though the HUST ACMICPC team shared their codes online, many organizations still have problems configuring their own machines, under those circumstances, _zhblue_'s service came in handy.

However Shang and I believed that _zhblue_'s service is legitimate business practices and it's beyond reproach, the fact that _zhblue_ doesn't belong to HUST and he's taking advantages of HUST's brand effect made the staff of HUST feel bad. I guess those who were feeling bad made the decision of removing acm.hust.edu.cn off their official hust.edu.cn domain.


### 1.5 The Purpose of This Case Study
As far as I'm concerned, HUST Online Judge is not a typical peer production project. In the very beginning, I believed there are many features that distinguish it from other projects, however, after I contrasted the motivation of this project to what I've learned about the "open source way", I found more and more similarities between them. All in all, it's very beneficial for me to have a deeper understanding of the "open source way". I'd like to discuss my findings of HUST Online Judge in the following parts.


## 2 Motivation
### 2.1 I Love It!
The initial contributors were the members of HUST ACMICPC team who joined HUST Online Judge developing team due to their fondness of coding and algorithm. "Programming for those people are similar to hobbies like swimming, playing football or watching movies", Shang said. Absolutely, this is an intrinsic motivation and it can result in high-quality learning and creativity[3].


### 2.2 I Need It!
Also, they wanted to have their own online judge which enabled them to better enjoy training algorithm. In a word, they thought they really need this system. To begin with, I assumed “I need it” is kind of intrinsic motivations because this feeling is an instinctive reaction from my standpoint. But later I realized that it's complex.

If they only wanted to train algorithm, they could simply buy one or keep using other online judges. The point is that they need their **own** online judge, and it's just like I don't want to use computers in the library and I need to have my own laptop. It can be both intrinsic and extrinsic. If they need their own online judge in that they can have more fun training, it's intrinsic. If they wanted to compete with other online judges, it's extrinsic. Nonetheless, Raymond proposed three basic motives, which are different from the intrinsic and extrinsic classification, one of them is that "they may directly benefit from the software and software improvements they develop, because they have a use for them"[4]. I think this motive best describe the participants of HUST Online Judge project.


### 2.3 Sense of Collective Honor
To quote Shang:
> They were proud to be students of HUST
> The HUST Online Judge helped expand the influence of HUST

Many HUST students later joined the Online Judge project out of their sense of belonging and their sense of collective honor. It's slightly different from typical "inner source"[5] because students receive no salary but they have stronger sense of identity. Besides the programming team, those HUST students who were using this system could offer suggestions and report bugs.

### 2.4 Utilizing the Influence
Indisputably, open software is the typical collaboration through open superposition. So there are .[6]


## 3 Differences
### 3.1 Benefits


### 3.2 Shortcomings


## 4 The Dilemma of Peer Production Inside A University

Comparing this project to a baby, she was born inside a university and then moving out of her parents' house when she could make a living. The












## References
[1]: Kurnia, A., Lim, A., & Cheang, B. (2001). Online judge. Computers & Education, 36(4), 299-315.

[2]: Anderson, C. (2009). Free: The future of a radical price. Random House.

[3]: Ryan, R. M., & Deci, E. L. (2000). Intrinsic and extrinsic motivations: Classic definitions and new directions. Contemporary educational psychology, 25(1), 54-67.

[4]: Raymond, E. (1999). The cathedral and the bazaar. Knowledge, Technology & Policy, 12(3), 23-49.

[5]: Dinkelacker, J., Garg, P. K., Miller, R., & Nelson, D. (2002, May). Progressive open source. In Proceedings of the 24th International Conference on Software Engineering (pp. 177-184). ACM.

[6]: Howison, J., & Crowston, K. (2014). Collaboration through open superposition. Mis Quarterly, 38(1), 29-50.
