# HOW TO ASK QUESTIONS
_How To Get Help Like A Boss_

:heavy_exclamation_mark:**PLEASE READ FULLY**:heavy_exclamation_mark:

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of Contents

- [INTRO](#intro)
- [General Structure Of The Question](#general-structure-of-the-question)
- [Before You Ask](#before-you-ask)
- [When You Ask](#when-you-ask)
  - [Approaches examples](#approaches-examples)
    - [Approach 1 (bad)](#approach-1-bad)
    - [Approach 2 (good)](#approach-2-good)
    - [Approach 3 (complex issue)](#approach-3-complex-issue)
    - [Approach 4 (even more complex issue)](#approach-4-even-more-complex-issue)
  - [Front-End Specific Tools To Use](#front-end-specific-tools-to-use)
- [Where To Ask](#where-to-ask)
- [Further Readings On The Topic](#further-readings-on-the-topic)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
<!-- generated with [DocToc](https://github.com/thlorenz/doctoc) -->

## INTRO
In the world of hackers, the kind of answers you get to your technical questions depends as much on the way you ask the questions as on the difficulty of developing the answer. This guide will teach you how to ask questions in a way more likely to get you a satisfactory answer.

**It sometimes looks like we're reflexively rude to newbies and the ignorant. But this isn't really true. Please try to ask good questions :smile_cat:**

## General Structure Of The Question

It is important to give your audience the proper context.
Luckily delivering context in software engineering
is much simpler than in many other fields.

_To get the best feedback on your issue,
please, follow the structure of asking below.
Of course wording can be different from suggested,
depending on your particular situation_

1. I am doing ..... (e.g. task name
   and a link to the complete task description)
1. I want to... (achieve something, e.g. have an element on a web page to float above other elements)
1. I tried this... (code fragment, or codepen with minimal yet sufficient code fragment to reproduce the issue)
1. How do I....? / What did I miss?

[_^ back to TOC^_](#table-of-contents)

## Before You Ask
Before asking a question, do the following:

1. If your question is about course - [FAQ](https://github.com/kottans/frontend/blob/master/faq.md).
2. If your question is about tasks -  good place to ask is either of our [chats](#where-to-ask).
3. If question is about JS or HTML/CSS - search Web, [MDN](https://developer.mozilla.org), etc.
4. Also you can find an answer by inspection or experimentation.
5. You're a programmer! So try to find an answer by reading the source code.

When you ask your question, display the fact that you have done these things first; this will help establish that you're not being a lazy sponge and wasting people's time. Better yet, display what you have learned from doing these things. We like answering questions for people who have demonstrated they can learn from the answers.

Take your time. Do not expect to be able to solve a complicated problem with a few seconds of Googling. Sit back, grab a cup of tea, relax and give the problem some thought before approaching experts. Trust us, they will be able to tell from your questions how much reading and thinking you did, and will be more willing to help if you come prepared. Don't instantly fire your whole arsenal of questions just because your first search turned up no answers (or too many).

Prepare your question. Think it through. Hasty-sounding questions get hasty answers, or none at all. The more you do to demonstrate that having put thought and effort into solving your problem before seeking help, the more likely you are to actually get help.

**Remember, [there is no such thing as a stupid question.](https://en.wikipedia.org/wiki/No_such_thing_as_a_stupid_question)**:wink:

[_^ back to TOC^_](#table-of-contents)

## When You Ask
* **Write in clear, grammatical, correctly-spelled language**
* **Use [Stack Overflow](https://stackoverflow.com/)** 

    _There are many similar questions, so try [SEARCH](https://stackoverflow.com/search?q=) first and then Ask._

* **Be precise and informative about your problem**

     Describe the symptoms of your problem or bug carefully and clearly.
     
     Describe the environment in which it occurs (for example a browser).
     
     Describe the research you did to try and understand the problem before you asked the question.
     
     Describe the diagnostic steps you took to try and pin down the problem yourself before you asked the question.

* **Describe the problem's symptoms, not your guesses**

* **Be explicit about your question**

[_^ back to TOC^_](#table-of-contents)

### Approaches examples

#### Approach 1 (bad)

A question like
> I am trying to fetch data from server and
> publish it on a web page, but nothing happens.
> What am I doing wrong?

requires too many clarifications and therefore
can be ignored by community.

[_^ back to TOC^_](#table-of-contents)

#### Approach 2 (good)

The alternative approach can be as follows.

> I am trying to fetch data from a server like this.
> ```
> const query = "https://api.somewhere.else/?id=5";
> let info;
> fetch(query).then(response => {
>   if (response.ok) {
>     return response.json();
>   }
>   throw Error('Querying ' + query + ' failed');
> }, reject => console.error(reject.message))
> .then(json => {
>   info = json.results;
>   return;
> });
> document.getElementById('output').innerHTML = info.name;
> ```
> `info` receives data from server response, but `output`
> element doesn't get updated as expected. What is my mistake?

The fragment above provides required and sufficient context
and experienced developer will figure out the problem instantly.

This approach requires a bit more efforts from the poster
namely copy-pasting a code fragment. But the response rate
will be much higher.

[_^ back to TOC^_](#table-of-contents)

#### Approach 3 (complex issue)

What if the fragment is way too big and also
UI render required to see the issue clearly?

Publish a [codepen](https://codepen.io/) or use
any other [similar service](#front-end-specific-tools-to-use).

Then post the link and your comments and question
to a community chat.

[_^ back to TOC^_](#table-of-contents)

#### Approach 4 (even more complex issue)

What if the project is way too big for codepen
and you cannot extract a part of it to build proper
visualization?

Just open a [draft pull request](https://github.blog/2019-02-14-introducing-draft-pull-requests/)
for the code review!
That's what draft pull requests can be efficiently used for.

You can open a PR in your own repository.
Put your code fragment in a dedicated branch, push,
publish the project (on e.g. GitHub Pages) and invite
others to review your code.

You may need to involve them as collaborators via
project settings. So, invite only those you trust,
and make sure they want to be invited.

[_^ back to TOC^_](#table-of-contents)

### Front-End Specific Tools To Use

**IF YOU USE ONE OF THESE TOOLS TO DISPLAY YOUR CODE YOU WILL GET MORE QUICK ANSWER.**
* **[CodePen](https://codepen.io/)**
* **[repl.it](https://repl.it/)**
* **[jsconsole](https://jsconsole.com/?q=console.log(%27AA%27))**

[_^ back to TOC^_](#table-of-contents)

## Where To Ask

1. [FE Students | Kottans](https://t.me/joinchat/DmX0JBHVkEhV1us2HdMmpA) - chat for students, where you can discuss anything related to the current course
2. [FE Questionarium | Kottans](https://t.me/joinchat/DmX0JAl-mh5W0jrWli8Ycw) - if you need a help of one of the mentors, or maybe from all of them simultaneously, you can ask it there

:heavy_exclamation_mark:_Please do **NOT** write code in the chat if this is more than 5 lines_:heavy_exclamation_mark:

Use [online services](#front-end-specific-tools-to-use) to post code instead.

:heavy_exclamation_mark:_Please do **NOT** post code as screenshots
as this may require your readers to re-type the code
to see how it would work_:heavy_exclamation_mark:

Many chat apps (e.g. Telegram) support markdown.
Put your code between `` ``` `` and `` ``` ``
(two rows containing triple backticks) to have
your code properly formatted.
`Shift` or `Alt` plus `Enter` keys allow you to write
multi-line chat message.

[_^ back to TOC^_](#table-of-contents)

## Further Readings On The Topic

If you want to know more details on the topic
or see how other sources discover it and what
they highlight on, consider reading any of the
below materials:

- [How To Ask Questions The Smart Way](http://www.catb.org/esr/faqs/smart-questions.html) -
  classics; :warning: suggests outdated tool, so be smart
  and just use contemporary replacement tools as appropriate
- [How do I ask a good question?](https://stackoverflow.com/help/how-to-ask) -
  the official Stack Overflow guide (5 minutes reading time)
- [Ten Tips For Asking Good Questions](https://www.dummies.com/careers/find-a-job/interviews/ten-tips-for-asking-good-questions/) -
  a really general guide yet applicable in any domain

[_^ back to TOC^_](#table-of-contents)
