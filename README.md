# Projects Rules for the Distributed Systems Course

[Giovanni Ciatto](mailto:giovanni.ciatto@unibo.it), [Andrea Omicini](mailto:andrea.omicini@unibo.it), and [Matteo Magnini](mailto:matteo.magnini@unibo.it)

## Overview

The exam consists of an oral discussion where students present a project of their choice, backed by a final report which must be submitted and validated before the discussion.

Generally speaking, a project consists of a study, design and implementation effort requiring about `90` hours _per person_ in total. 
A project may be designed and implemented by a __group__ of cooperating students. 
The maximum size for a group is `3` people—`4` people in exceptional and well-motivated cases. 
In this case, the required effort is expected to __scale up linearly__ with the amount of students composing the group, which means about `90 * N` hours, being `N` the amount of students in a group. 
In any case, a __final report__ is expected to be produced for each project, (possibly) during its development. 
In case of a group project, the final report can be shared (i.e. __unique__) but it is required to __explicitly__ state how the work was split among the members of the group. 
Finally, students will have to __discuss__ their project in order for them to be assessed. 
Assessment is always individual, even in case of a group of students jointly participating to the same project.

Students may either reserve a project among the ones we propose on the [Project Proposals Page] or propose one proactively. 
In both cases they will have to open a new conversation on the [Projects Forum] in order to either reserve or propose a project. 
Since then, any discussion concerning the project must will be held within that conversation—there including __submission__.
Projects proposed by students need to be __explicitly approved__ by one of the teachers in order for them to be considered valid. 
The teacher approving the project is usually the one that will supervise the work and assess it once it is over.

__Worker students__, non-italian-speaking students, or students having some other sort of special need, may ask to renegotiate the terms of the examination.
In this case, students can send a _private_ email to <andrea.omicini@unibo.it>, adding all other teachers __in copy__.

## Procedure 1: Reserving a project

Students – either as individuals or as groups – may reserve a project by __opening a new conversation__ on the [Projects Forum].

_Plase use the following naming convention for conversations:_
```
[Surname1, Surname2, ..., SurnameN] Project reservation: <brief activity name>
```

The reservation post must specify at least:
1. a reference to the chosen project,
2. the members composing the team (in case of a team),
3. the _extimated_ starting date for the project, and
4. some strict temporal constraint, if any
    - e.g. someone in the group is going to graduate soon

> We may __reject__ project reservation requests involving projects which have already been reserved/completed by your colleages, either in the current accademic year or in some previous one. So, please double-check your colleagues requests/proposals before submitting your reservation request.
> Consider having a look to these pages for double-checking:
> - [APICe SD Projects along the years]
> - [Projects Forum]

> In case of conflict with some previous project, feel free to submit your reservation request anyway, asking for a _negotiation_ of a similar project.

## Procedure 2: Proposing a project

Students are allowed – and actually kindly invited – to propose a project by __opening a new conversation__ on the [Projects Forum].
In doing so, proposers need to describe:
- their __vision__, i.e. what they want to realise
- their __learning goals__, i.e. why they believe the proposed project is interesting for the course and what they expect to learn
- the __deliverable__ they intend to produce (application, library, presentation, etc)
- in case the deliverable consists of some _software artifact_, a description of the __usage scenarios__ for the software 

It is ok to initially provide a raw description of your idea, ask for feedback, and provide the aforementioned information later.

_Plase use the following naming convention for conversations:_
```
[Surname1, Surname2, ..., SurnameN] Project proposal: <brief activity name>
```

Proposals must be __explicitly accepted__ by one of the teachers before the students may proceed with Procedure 3.

The teachers may also suggest some edits to the proposed project in order for it to be approved.

Acceptance – as well as denials, or suggestions – will be communicated on the same conversation opened by students.

> We may __reject__ project proposals involving projects which have already been reserved/completed by your colleages, either in the current accademic year or in some previous one. So, please double-check your colleagues requests/proposals before submitting your reservation request.
> Consider having a look to these pages for double-checking:
> - [APICe SD Projects along the years]
> - [Projects Forum]

> In case of conflict with some previous project, feel free to submit your proposal anyway, asking for a _negotiation_ of a similar project.

## Procedure 3: Beginning a project

Before actually start working on a project, students will have to:

1. produce an (very short, 1-2 pages) __initial report__, specifying:
    1. a __title__ for the project
    0. an __abstract__ for the project (max 2000 chars), briefly summarising the goal of the project
    0. a section __extensively describing__ the _goals_ and _expected deliverables_ of the project, along with their __requirements__
    0. a section describing the __expected work plan__, and the __expected division of labour__ in case of a group

    > (such a report can be written using either __Markdown__ or __LaTeX__, and it can eventually be extended to become the _final report_)

    > (notice that the aforementioned information are allowed to change during the project development)

2. post the initial report on the project conversation on the [Projects Forum]
    - the conversation is assumed to exists at this point because of Procedure 1-2

3. wait for the teachers' approval or suggestions
    - upon approval, teachers will provide:
        - a Git repository for the project
        - an Apice Web page for the project

After receiving a Git repository, students can start working at their project.
Committing and pushing frequently is recommended.

### About the initial report

The workflow described above is aimed to:
- make students aware of what they should do BEFORE doing it
- ease our projects management activities
- prevent the loss of the produced knowledge or code, making your projects potentially useful for the future students.

In particular, the initial report is the most valuable artifact in this phase.
Within the initial report, students must take care of specifying their goals in a clear, precise, undambigous, and __incremental__ way.

> Project assessment will take __goals satisfaction__ into account: it is important that your projects satisfy the goals that you have chosen

Negotiation of the initial report is aimed at helping the students in the selection and formalisation of __reasonable goals__

> By submitting an initial report students __commit__ to the goals therein described

However, we are aware that issues may arise while working on a project.
For this reason, it is important to describe goals in an __incremental__ way.
In some significant issues arise, students may ask to renounce to the satisfaction of some goals---provided that minimal pool of goals has already been satisfied.

## Procedure 4: Project design & development

Students are assumed to properly design and develop the projects they have chosed, producing quality code to be tracked by means of the provided GitLab repository.

They are encouraged to use some structured workflow during the development, like for instance:
- the [GitLab flow](https://docs.gitlab.com/ee/topics/gitlab_flow.html), which may be sufficient in this context
- or the well-known [Git flow](https://it.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow), which is slightly more complicated, but also more popular and used in the real world

This is mandatory in case of a group.

Students are encouraged to keep track of their design and architectural choices by __progressively__ extending the initial report. 
They are __discouraged__ from filling the report with (too much) code: the report must track ideas and choices, design and architectures, but the code must NOT be its main content.

Students are encouraged to adopt a __test-driven__ and __model-first__ approach, when possible: they are going to be __engineers__, not programmers.
This means that automatic tests should be designed and written along with interfaces, and __before__ implementation.

> Students are encouraged to exploit [GitLab's "Issues" feature](https://docs.gitlab.com/ee/user/project/issues/) during the development process, in particular when:
- discussing the implementation of a new idea
- submitting feature proposals
- reporting bugs and malfunction
- elaborating new code implementations

> If an apparently unsolvable technical or organizational problem arises, students are encouraged to first try to solve it autonomously and, in case of failure, ask for help to teachers, either within some GitLab issue (for what concerns technical aspects) on the [Projects Forum].

### About the Git repository

Despite not strictly required for the course, please take care of keep your repository clean.
This involves:
- correctly setting up your `.gitignore`
- fill up the `README.md` file in a meaningful and informative way
- avoid tracking binary files, dependencies, or IDE configuration files

Finally, take care of making the last version of your code available on the `master` or `main` branches.

### About Build Automation

In case your project involves the production of software artifacts, it is __mandatory__ to leverage some __build automation system__.

There are no constraint on the particular build automation system, but keep in mind that each programming platform comes with its preferred build automation systems:
- Maven or Gradle for the Java, Kotlin, Scala
- Sbt for Scala
- NPM for JS projects
- Pip for Python projects
- Make for C
- etc

> It is ok to develop your project in some language different from Java, but in that case it is __your responsibility__ to select the most adequate build automation technology .

Please endow your codebase with adequate __unit test__ suites, possibly runnable with a single command, via the build automation tool of choice.

Setting up a continous integration pipeline running the tests as frequently as possible is strongly encouraged as well.

## Procedure 5: Project discussion

Students must __explicitly communicate__ to the project supervisor their intention to discuss the project, by adding a new post on the project conversation on the [Projects Forum], and by __attaching the final report__. 
The supervisor will then propose an appointment for the discussion, provided that the final report is satisfying.
Otherwise the supervisor may propose some improvements.
In this case, students will have to produce an improved version of the final report and post if again, __without removing or replacing the previous version__.

Before admitting the students to the project discussion, the supervisor will take care of assessing their lab activity.
This may involve the scheduling of another meeting with the supervisor to discuss the lab activity.

> Summarising, students are admitted to the final discussion with prof. Omicini only after they (i) have submitted a final report, (ii) have submitted their lab activity, and (iii) both the final report and the lab-activity have been assessed by some supervisor.

During the discussion, the professor will test the students' knowledge about the project topic, and, possibly, __its connection to the other topics presented within the course__. 
In case of a group project, the individual knowledge and contribution will be tested. 
The professor will also quickly test the quality of the produced report and code. 

### About the final report

The final report must be correctly written (either in Italian or in English) and it must be a meaningful but brief (up to ~50 pages) guide to the topic studied during the project.

The admissible formats are:
- Markdown (template [here](./final-report-template.md))
- Latex (template [here](https://www.overleaf.com/read/thjtqmskvzcs))

The provided templates are just suggestions and their structure is _not_ the only admissible one.

[Project Proposals Page]: <https://github.com/gciatto-unibo/sd-project-proposals>
[Projects Forum]: https://virtuale.unibo.it/mod/forum/view.php?id=918628
[APICe SD Projects along the years]: https://apice.unibo.it/xwiki/bin/view/Courses/SdProjects
