# Adaptation Paper: The HUST Online Judge
#### Instructor: James Howison
#### Student: Sifan Guo

## 1 Introduction
### 1.1 People Who Started This Project
About 10 years ago in 2008, _Sempr_, a former member of Huazhong University of Science and Technology([HUST](https://en.wikipedia.org/wiki/Huazhong_University_of_Science_and_Technology)) [ACM/ICPC](https://en.wikipedia.org/wiki/ACM_International_Collegiate_Programming_Contest) team, had an idea of building an online judge[1] both for their team's algorithm training and for his own graduation project. Although many successful projects are created by a single person, more people are needed in order to perfect them. According to one former participant Shang(my interviewee), before _Sempr_ began coding, _Sempr_ discussed this idea with his teammates and the team's advisors, and undoubtedly, they all encouraged him and promised to offer help when needed. Through the efforts of all these people, the HUST Online Judge first came out with the domain acm.hust.edu.cn which was no longer used after Jan 2018 due to many reasons.


### 1.2 Embracing the Wonderful GPL v2 License!
It was no later than a week after HUSTOJ started its service when the team decided to share their codes on [Google Code](https://code.google.com/archive/p/hustoj/) under the GNU General Public License, version 2. Shang told me that their team made this decision for many reasons:

1. Their teammates were all busy training and the fact that they were good at algorithms doesn't necessarily mean they were capable of programming. They all agreed that they could turn to more people for help.

2. The online judge was good enough for them, and they want more users to join and offer feedbacks because different people would have different viewpoints which could help them to improve the online judge in various ways.

3. Most contributors of this project were senior students, and they were afraid of being too busy to continue contribution after the graduation.

4. They are using Subversion([SVN](https://subversion.apache.org)) to track versions, and they thought that this can encourage more people to contribute codes in that if everyone can see the contribution history, people are more likely to share their skills.[2]

5. As mentioned in the second reason, they thought highly of their online judge, so they wanted to share their codes with the world and "show off".

6. The staff of HUST considered it as a great way to expand the influence of the university, also, this can be counted as their working achievements.


### 1.3 Becoming Popular
As more and more universities began to have teams for ACM/ICPC, they attached great significance to building their own online judge system because they can customize the system and flexibly host their own competitions. Including many high schools, 126 organizations (most of them are universities: [check the whole list here](https://code.google.com/archive/p/hustoj/)) throughout the world had used the HUST Online Judge or designed their own system based on it. According to Shang, HUST Online Judge was well-known to domestic ACM/ICPC teams then. In a word, it was definitely a successful project around 2010.


### 1.4 The Purpose of This Case Study
As far as I'm concerned, HUST Online Judge is not a typical peer production project. In the very beginning, I believed there are many features that distinguish it from other projects, however, after I contrasted the motivation of this project to what I've learned about the "open source way", I found more and more similarities between them. All in all, it's of great benefit for me to have a deeper understanding of the "open source way". I'd like to discuss my findings of HUST Online Judge in the following parts.


## 2 Motivations of HUST Students
### 2.1 I Love It!
The initial contributors were the members of HUST ACM/ICPC team who joined HUST Online Judge developing team due to their fondness of coding and algorithm. "Programming for those people is similar to hobbies like swimming, playing football or watching movies", Shang said. Absolutely, this is an intrinsic motivation and it can result in high-quality learning and creativity[3].


### 2.2 I Need It!
Also, the initial contributors wanted to have their own online judge which enabled them to better enjoy training algorithm. In a word, they thought that they really need this system. To begin with, I assumed “I need it” is kind of intrinsic motivations because this feeling is an instinctive reaction from my standpoint. But later I realized that it's more complex than I thought.

If they only wanted to train algorithm, they could simply buy one system or keep using other online judges. The point is that they need their **own** online judge, and it's just like I don't want to use computers in the library and I need to have my own laptop. It can be both intrinsic and extrinsic.

On the one hand, if they need their own online judge in that they can have more fun training, it's more intrinsic. On the other hand, if they wanted to compete with other online judges, it's more extrinsic. Nonetheless, Raymond proposed three basic motives, which are different from the intrinsic and extrinsic classification. The first one of them is that "they may directly benefit from the software and software improvements they develop, because they have a use for them"[4]. I think this best describes the participants of HUST Online Judge project.


### 2.3 Sense of Collective Honor
To quote Shang:
> They were proud to be students of HUST
>
> The HUST Online Judge expanded the influence of HUST

Many HUST students later joined the Online Judge project out of their sense of belonging and collective honor. It's slightly different from typical "inner source"[5] because students receive no salary as reward but they have stronger sense of identity. Besides the programming team, those HUST students who were using this system could offer suggestions and report bugs.

## 3 Motivations of Participants From Other Organizations
According to the [GNU General Public License, version 2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html), users of HUST Online Judge codes are not required to participate the project. However there were still many participants who came from other organizations, most of them are not as famous as HUST in China. Moreover, they didn't need to customize the online judge themselves, instead, they totally relied on HUST Online Judge to update theirs. Also, lacking software engineers is another possible reason why they didn't start their own online judge repository.

In my opinion, they need to use HUST Online Judge and it's the most convenient way, hence, they directly benefited from this project just like the HUST students. Furthermore, HUST students might think that they deserve using this system, whereas participants from other organizations might feel grateful. So their motivations are likely to be a) they were using it so they wanted to improve it and b) the desire to give back to the community, otherwise known as reciprocity[6].

Besides the volunteers, there were some groups of contributors who sold their services to HUST Online Judge users. Even though I can't claim that they're participating this project with the idea of making money, I insist that a business opportunity could make _One Time Code Contributors_[6] become _sustained contributors_[7]. And this is beneficial for the project in the long run. So seeking for financial rewards could be a possible motivation.


## 4 From SVN to GIT
HUST Online Judge was using Subversion([SVN](https://subversion.apache.org)) between 2008 and 2014. Since Google Sites had been blocked in 2011(data from [here](https://en.wikipedia.org/wiki/Websites_blocked_in_mainland_China)), more and more users were complaining about the inconvenience of using _google code_. Eventually the contributors decided to start using github with [GIT](https://git-scm.com), and they are still using GIT till now.

It's worth noting that they were using an automatic mirroring tool called [svn2github](http://svn2github.com) to clone the SVN repository to GitHub. When it comes to version control, both tools are awesome. As far as I know, there is no significant difference between SVN and GIT regarding collaboration infrastructure especially when this is a software development project. Yet there are differences between them, GIT is more efficient because we can commit, merge and practically do anything offline, while SVN is easier to learn.



## 5 Without the Domain hust.edu.cn, What Would HUST Online Judge Be?
After Jan 2018, the origin domain acm.hust.edu.cn was no longer used after nearly 10 years of service. There are two websites -- [hustoj.org](http://www.hustoj.org) and [hustoj.com](http://www.hustoj.com/), both of them claimed to be HUST Online Judge but neither provides the real judging service as acm.hust.edu.cn used to. The [hustoj.org](http://www.hustoj.org) offers English version and works as a backup which retains the original data but submission hasn't been enabled yet. On the other hand, [hustoj.com](http://www.hustoj.com/) does provide demo submission and judging service, however, unlike the original non-profit service, it seems to be a commercial website whose purpose is selling the customer service. It's a wonderful business mode[8] but not a university service as it should be.

I asked Shang why the domain was changed and he indicated that it's the university's decision. In addition, he said we doesn't know the real reasons why the university decided not to offer her domain and servers anymore. I tried to contact the staff by email but no one responded yet, as a result, what I'm going to say are all based on my conjecture, **please don't hesitate to let me know by pulling request or adding issues, if anyone has the other stories of HUST Online Judge. I'll be more than happy to update this paper in no time.**

After in-depth discussion with Shang, we both agreed the commercialization of HUST Online Judge would be direct cause. Most Chinese universities would only offer online services or other alike resources to their students for academic use, otherwise things would become much more complicated because applying for commercial projects requires approval of many departments of the university. In other words, if we're making money by using resources of the organization without supervision, it's like cheating. Case in point, an active contributor of HUST Online Judge and also the administrator of [hustoj.com](http://www.hustoj.com/) _zhblue_ is selling his service. Although _zhblue_ is not from HUST, he did play an irreplaceable role in promoting HUST Online Judge by offering paid service. Because even though the HUST ACM/ICPC team shared their codes online, many organizations still have problems configuring their own machines, under those circumstances, this kind of services came in handy.

Although Shang and I considered that _zhblue_'s service is legitimate business practices and it's beyond reproach, the fact that _zhblue_ doesn't belong to HUST and he's taking advantages of HUST's brand effect might make the HUST staff feel bad. I guess those who were feeling bad made the decision of removing acm.hust.edu.cn off their official hust.edu.cn domain. Frankly speaking, I have no idea of what would HUST Online Judge be without the domain hust.edu.cn, because the hust.edu.cn domain is like HUST's trademark and so does almost every university(See more: [ACM OJ Collection](http://www.cnblogs.com/Xredman/archive/2009/03/23/1420015.html)).

After all, those who are funding a project would think about tradeoff, given that they are not altruistic. In the Part 4 of this paper, I claimed the governance mode is no different from the typical "open source way", however, like _inner source_, the organization's influence can't be ignored. But luckily, this sort of influence wouldn't affect the collaboration mechanism, because HUST staff didn't participate in writing codes, which means their decisions could only have effect on the external attributes of the project other than the codes. For instance, even though HUST Online Judge was no longer serving within hust.edu.cn domain, the project itself both the codes and the contribution history remain in the github unmodified.


## 6 Other Observations
Indisputably, open software development project is the typical successful collaboration through open superposition[9]. So this project is by no means difficult to be distributed. Most high schools that used HUST Online Judge's codes are likely to contribute codes and report bugs, whereas some universities preferred to build their own online judges based on HUST's and later they only contribute codes to their repositories. Using the terminology of github, these universities had **forked** the HUST Online Judge project but they chose not to click the **pull request**. Indeed, some HUST students argued that it's unfair. However, as I've learned more about open source world, from Karl's[10] standpoint, this is not only beyond reproach, but also it makes open source prevalent. Because every new repository forked from HUST Online Judge can influence more people as long as they followed the GPL license. As for HUST initial contributors, I think the moment when they shared their codes, they deserved to be honored, and being honored is the best reward, isn't it?



## References
[1]: Kurnia, A., Lim, A., & Cheang, B. (2001). Online judge. Computers & Education, 36(4), 299-315.

[2]: Shah, S. K. (2006). Motivation, governance, and the viability of hybrid forms in open source software development. Management science, 52(7), 1000-1014.

[3]: Ryan, R. M., & Deci, E. L. (2000). Intrinsic and extrinsic motivations: Classic definitions and new directions. Contemporary educational psychology, 25(1), 54-67.

[4]: Raymond, E. (1999). The cathedral and the bazaar. Knowledge, Technology & Policy, 12(3), 23-49.

[5]: Dinkelacker, J., Garg, P. K., Miller, R., & Nelson, D. (2002, May). Progressive open source. In Proceedings of the 24th International Conference on Software Engineering (pp. 177-184). ACM.

[6]: Lee, A., Carver, J. C., & Bosu, A. (2017, May). Understanding the impressions, motivations, and barriers of one time code contributors to FLOSS projects: a survey. In Proceedings of the 39th International Conference on Software Engineering (pp. 187-197). IEEE Press.

[7]: Crowston, K., & Fagnot, I. (2018). Stages of motivation for contributing user-generated content: A theory and empirical test. International Journal of Human-Computer Studies, 109, 89-101.

[8]: Anderson, C. (2009). Free: The future of a radical price. Random House.

[9]: Howison, J., & Crowston, K. (2014). Collaboration through open superposition. Mis Quarterly, 38(1), 29-50.

[10]: Fogel, K. (2017). Producing open source software: How to run a successful free software project. Version: 2.3106. Retrieved from (https://producingoss.com).
