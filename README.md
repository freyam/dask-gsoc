# My GSoC Application for Dask

<p align="center">
  <img Dask width="500" height="500" src="https://docs.dask.org/en/latest/_images/dask_icon.svg">
</p>

## **My Proposal** [**`dask-proposal-freyam.md`**](https://github.com/freyam/dask-gsoc-application/blob/main/dask-proposal-freyam.md)

<br>

## Visualizing performance characteristics of computations ([link](https://github.com/dask/dask/wiki/GSOC-2021-Project-Ideas))

**Potential Mentors:** [Genevieve Buckley](https://github.com/GenevieveBuckley/) and [Martin Durant](https://github.com/martindurant)

**Description:** Dask users are sometimes caught off guard when they have a computation that works well and then add a new step which results in an overall computation with very different performance characteristics. We'd like to build better visualization tools so that users can more easily identify possible areas of inefficiency in their computations.

**Expected Skills:** A good candidate would be familiar with Python, and have some experience reasoning about Python performance. Experience with HTML and JS graph visualization libraries would be a plus, but not a requirement.

**Relevant community discussion**

* https://github.com/dask/dask/issues/7141
* https://github.com/dask/dask/issues/7301

## Abstract

One of Dask's primary functions is to construct task graphs and optimize them before decorating the functions to operate lazily. By looking at the **interconnectedness of tasks**, one can learn more about potential bottlenecks where parallelism may or may not be possible to apply to simplify the task graph further.

Dask currently uses `graphviz` to render a task graph. The `.visualize` method and the `dask.visualize` functions are simple and effective. They generate a static black-and-white image showing the blocks and their connections. However, the task graph struggles to work with complex computations and doesn't give a clear idea about the feasibility of the tasks. There's a scope of improvement here.

I plan to **color code the graph and highlight the room for optimization** (`dask.optimization`). This allows the user to learn more about the program's performance characteristics and distinguish how the computation fares at a higher complexity. I also plan to introduce **collapsible blocks that group smaller blocks into a single large block**. This simplifies the rendered graph, especially when the crucial data contains a large number of nodes.



## Dask Guidelines ([link](https://github.com/dask/dask/wiki/Google-Summer-of-Code-Student-Instructions))

### Me the me

- [x] Your full name
- [x] University / current enrollment
- [x] Short bio / overview of your background
- [x] How can we contact you?
  - [x] Email
  - [x] GitHub username
  - [x] Any other username you want us to know about

### Me the programmer

- [x] In your project proposal let us know about your programming experience.
- [x] What is your experience programming? Tell us about something you have created.
- [x] What is your experience with Python?
- [x] Have you ever used git or another version control system? Do you have experience using GitHub?
- [x] What is your experience with Open Source? Have you ever contributed to another open source project?

### Project Description

- [x] What do you want to achieve?
- [x] What excites you about this project? Why did you choose it?
- [x] What qualifications do you have to implement your idea? Why are you suited to work on this project?
- [x] How much time do you plan to invest in the project before, during, and after the Summer of Code? (we will expect full time 40h/week during GSoC). If you plan to take any vacations over the summer, let us know about it here.
- [x] How will you break your project into smaller tasks? Please provide a schedule of how time will be spent on sub-tasks of the project over the GSoC development period. While we will not hold you to this schedule, this lets us know that you have thought about how to break the project into smaller tasks and will help us monitor your progress throughout the summer.
- [x] Please also note in the schedule where could formulate a pull request. These would be points where you can have a self contained, documented, and tested piece of functionality. Doing this at several points during the summer helps to keep code reviews manageable. A big pull request at the end of the summer will likely be hard to review and merge before the project deadline.

## NumFOCUS Guidelines ([link](https://github.com/numfocus/gsoc/blob/master/CONTRIBUTING-students.md))

- [x] Have you communicated with the organization's mentors?
- [x] Have you communicated with the community?
- [x] Did you reference projects you coded WITH links to repos or provided code?
- [x] Did you provide several methods to contact you? (email, skype, mobile/phone, twitter, chat, and/or tumblr if available)
- [x] Did you include a preliminary project plan (before, during, after GSoC)?
- [x] Did you state which project you are applying for and why you think you will end up completing the project?
- [x] Do you have time for GSoC? This is a paid job! State that you have time in your motivation letter, and list other commitments!
- [x] Did you add a link to ALL your application files to a cloud hoster like GitHub or Dropbox? (easy points! wink)
- [x] Be honest! Only universal Karma points.
- [x] Did you create a pull request on the existing code?
- [x] Did you continue communication until accepted students are announced?
