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

4. They are using Subversion([SVN](https://subversion.apache.org)) to track versions, and this can encourage more people to contribute codes in that everyone can see the contributors.

5. As mentioned in the second reason, they thought highly of their online judge, so they wanted to share their codes with the world and "show off".

6. The staff of HUST considered it as a great way to expand the influence of the university, also, this can be counted as their working achievements.


### 1.3 Becoming Popular
As more and more universities began to have teams for ACMICPC, they attached great significance to building their own online judge system because they can customize the system and flexibly host their own competitions. Including many high schools, 126 organizations (most of them are universities: [check the whole list here](https://code.google.com/archive/p/hustoj/)) throughout the world had used the HUST Online Judge or designed their own system based on it. According to Shang, HUST Online Judge was well-known to domestic ACMICPC teams then. In a word, it was definitely a successful project around 2010.


### 1.4 Without the Domain hust.edu.cn, What Would HUST Online Judge Be?
After Jan 2018, the origin domain acm.hust.edu.cn was no longer used after nearly 10 years of service. There are two websites -- [hustoj.org](http://www.hustoj.org) and [hustoj.com](http://www.hustoj.com/), both of them claimed to be HUST Online Judge but neither provides the real judging service as acm.hust.edu.cn used to. The hustoj.org offers English version and works as a backup which retains the original data but submission hasn't been enabled yet. On the other hand, hustoj.com does provide demo submission and judge service, however, unlike non-profit service, it seems to be a commercial website which is selling the customer service[2].

I asked Shang why the domain was changed and he indicated that it's the university's decision. In addition, he said we can't know the real reasons which made the university decide not to offer her domain and servers anymore. I tried to contact the staff but no one responded, as a result, what I'm going to say are all based on my conjecture, **please don't hesitate to let me know by pulling request or adding issues, if anyone has the other stories of HUST Online Judge. I'll be more than happy to update this paper in no time.**

After in-depth discussion with Shang, we both agreed the commercialization of HUST Online Judge would be direct cause. In most Chinese universities, they are only allowed to offer online services or other alike resources to their students for academic use only, otherwise things would become too complicated because applying for commercial projects requires approval of many departments of the university. In other words, if we're making money by using resources of the organization without supervision, it's like cheating. Case in point, an active contributor of HUST Online Judge and also the administrator of hustoj.com _zhblue_ is selling his service. Although _zhblue_ is not from HUST, he did play an irreplaceable role in promoting HUST Online Judge by offering paid service. Because even though the HUST ACMICPC team shared their codes online, many organizations still have problems configuring their own machines, under those circumstances, _zhblue_'s service came in handy.

However Shang and I believed that _zhblue_'s service is legitimate business practices and it's beyond reproach, the fact that _zhblue_ doesn't belong to HUST and he's taking advantages of HUST's brand effect made the staff of HUST feel bad. I guess those who were feeling bad made the decision of removing acm.hust.edu.cn off their official hust.edu.cn domain.


### 1.5 The Purpose of This Case Study
As far as I'm concerned, HUST Online Judge is not a typical peer production project. In the very beginning, I believed there are many features that distinguish it from other projects, however, after I contrasted the motivation of this project to what I've learned about the "open source way", I found more and more similarities between them. All in all, it's very beneficial for me to have a deeper understanding of the "open source way". I'd like to discuss my findings of HUST Online Judge in the following parts.


## 2 Motivations of HUST Students
### 2.1 I Love It!
The initial contributors were the members of HUST ACMICPC team who joined HUST Online Judge developing team due to their fondness of coding and algorithm. "Programming for those people are similar to hobbies like swimming, playing football or watching movies", Shang said. Absolutely, this is an intrinsic motivation and it can result in high-quality learning and creativity[3].


### 2.2 I Need It!
Also, the initial contributors wanted to have their own online judge which enabled them to better enjoy training algorithm. In a word, they thought that they really need this system. To begin with, I assumed “I need it” is kind of intrinsic motivations because this feeling is an instinctive reaction from my standpoint. But later I realized that it's complex.

If they only wanted to train algorithm, they could simply buy one or keep using other online judges. The point is that they need their **own** online judge, and it's just like I don't want to use computers in the library and I need to have my own laptop. It can be both intrinsic and extrinsic. If they need their own online judge in that they can have more fun training, it's intrinsic. If they wanted to compete with other online judges, it's extrinsic. Nonetheless, Raymond proposed three basic motives, which are different from the intrinsic and extrinsic classification, one of them is that "they may directly benefit from the software and software improvements they develop, because they have a use for them"[4]. I think this motive best describe the participants of HUST Online Judge project.


### 2.3 Sense of Collective Honor
To quote Shang:
> They were proud to be students of HUST
> The HUST Online Judge helped expand the influence of HUST

Many HUST students later joined the Online Judge project out of their sense of belonging and their sense of collective honor. It's slightly different from typical "inner source"[5] because students receive no salary but they have stronger sense of identity. Besides the programming team, those HUST students who were using this system could offer suggestions and report bugs.

## 3 Motivations of Participants From Other organizations
According to the [GNU General Public License, version 2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html), users of HUST Online Judge codes are not required to participate the project. However there were still many participants who came from other organizations, most of them are not as famous as HUST in China. Moreover, they didn't need to customize the online judge themselves, instead, they relied on HUST Online Judge to update theirs. Also, lacking software engineers is another reason why they didn't start their own online judge repository.

In my opinion, they need to use it and it's the most convenient way, hence, they directly benefited from HUST Online Judge project just like the HUST students except that they came from other organizations. So their motivations are a) they were using it so they wanted to improve it and b) the desire to give back to the community, otherwise known as reciprocity[6].

Besides the volunteers, there were some groups of contributors who sold their services to HUST Online Judge users. Even though I can't claim that they're participating this project with the idea of making money, I insist that a business opportunity could make _One Time Code Contributors_[6] become _sustained contributors_[7].


## 4 From SVN to GIT
HUST Online Judge was using Subversion([SVN](https://subversion.apache.org)) between 2008 and 2014. Since Google Sites had been blocked in March, 2011(data from [here](https://en.wikipedia.org/wiki/Websites_blocked_in_mainland_China)), more and more users were complaining about the inconvenience. Eventually they decided to start using [GIT](https://git-scm.com) till now. It's worth noting that they were using an automatic mirroring tool called [svn2github](http://svn2github.com) to clone SVN repos to GitHub. When it comes to version control, both tools are awesome. Yet there are differences between them, GIT is more efficient because we can commit, merge or practically do anything offline, while SVN is easier to learn.






## 5
Indisputably, open software is the typical successful collaboration through open superposition[8]. So this project is by no means difficult to be distributed. Most high schools that used HUST Online Judge's codes are likely to contribute codes and report bugs, whereas some universities preferred to build their own online judges based on HUST's and later they only contribute codes to theirs. Using the terminology of github, these universities had **forked** the HUST Online Judge project but they chose not to **pull request**. Not only it is beyond reproach, but also it makes open source prevalent[9].

Comparing this project to a baby, she was born inside a university and then moving out of her parents' house when she could make a living. The












## References
[1]: Kurnia, A., Lim, A., & Cheang, B. (2001). Online judge. Computers & Education, 36(4), 299-315.

[2]: Anderson, C. (2009). Free: The future of a radical price. Random House.

[3]: Ryan, R. M., & Deci, E. L. (2000). Intrinsic and extrinsic motivations: Classic definitions and new directions. Contemporary educational psychology, 25(1), 54-67.

[4]: Raymond, E. (1999). The cathedral and the bazaar. Knowledge, Technology & Policy, 12(3), 23-49.

[5]: Dinkelacker, J., Garg, P. K., Miller, R., & Nelson, D. (2002, May). Progressive open source. In Proceedings of the 24th International Conference on Software Engineering (pp. 177-184). ACM.

[6]: Lee, A., Carver, J. C., & Bosu, A. (2017, May). Understanding the impressions, motivations, and barriers of one time code contributors to FLOSS projects: a survey. In Proceedings of the 39th International Conference on Software Engineering (pp. 187-197). IEEE Press.

[7]: Crowston, K., & Fagnot, I. (2018). Stages of motivation for contributing user-generated content: A theory and empirical test. International Journal of Human-Computer Studies, 109, 89-101.

[8]: Howison, J., & Crowston, K. (2014). Collaboration through open superposition. Mis Quarterly, 38(1), 29-50.

[9]: Fogel, K. (2017). Producing open source software: How to run a successful free software project. Version: 2.3106. Retrieved from [producingoss.com](https://producingoss.com).
