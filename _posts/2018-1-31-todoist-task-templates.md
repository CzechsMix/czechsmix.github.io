---
layout: post
title: How Todoist (Perhaps Unintentionally) Gave Us Task Templates
tags: [Productivity, Todoist]
---

If you follow me on [Twitter](https://twitter.com/sam_ferree), it's no secret I'm a huge fan of [Todoist](https://todoist.com). So you can expect posts like this one to come up from time to time. In this post, I explain how I've been using features of Todoist to implement what I call "Task Templates", But first things first...

# Project Templates and their drawbacks

While there is an existing feature known as templates, it is project based, and has some drawbacks. Task Templates are an alternative method for using templates in todoist, with some features that make them more desirable than project templates. Task Templates aren't explicitly a feature of Todoist, but a serendipitous result of four other Todoist features. Before we dive into Task Templates, let's look a little bit at Project Templates.

### Project Templates allow you to export an entire project to a csv file.

This file can then be imported back into Todoist as a new project. Project templates also have a feature known as relative dates. If you export a project with this enabled, the file will store "tomorrow" as "+1 day", so that when the project is re-imported the date of the tomorrow task isn't set to one day after whenever the project was originally exported.

### Project templates have some problems

This is an unfortunate consequence of the way they are stored, as a file. First your templates can't be stored easily in Todoist, they need to be stored on a device's file system. You can attach them as files to another task, or store them in another cloud service like google drive, but due to how the import process works, you would need to download that file down to your device, and then push it back up into Todoist.

Additionally, If you update a project template, you need to update the physical file, wherever you've stored it. 

# Why we can make Task Templates

Remember I said that Task Templates are just the product of four other key features? Let's go over what those are.

### Tasks can have sub-tasks.

The means that you can represent any project, as a task. Simply make all the tasks of a project a sub task of a task that as the same title as the project.

![Sub Tasks][sub_tasks]

### You can use the asterisk (\*) or colon (:) to make a task an un-checkable section header

Tasks starting with an asterisk and then a space don't get a checkbox. This is commonly used as a section header, but since it's still a task, it can still have sub-tasks. As a sidenote here, I like to also surround the task text in two additional asterisks (\*\*) so as to make the font bold.

![Section Header Edit][section_header_edit]

![Section Header][section_header]

### You can select and perform operations on multiple tasks

You can grab a range of tasks by holding down the shift key and click on the first and last task, or you can select tasks one at a time by clicking on them while holding the ctrl key. Once you have multiple tasks selected you can move them to a new project, add labels to them, set their priority, and several other operations.

![Multi Select][multi_select]

### Tasks can be duplicated.

The real kicker here is that when you duplicate a task, Todoist will also duplicate any of that task's sub-tasks. 

![Duplicate][duplicate]

# Making and using Task Templates

### First, Create an uncheckable task, and add sub tasks under it.

Let's say I'm making a very simple template for baking cookies. I prepare these often for parties and potlucks, and want a template ready that includes not only the steps to make the cookies, but also the adds the items to my grocery list (Which you also mange in Todoist right?) I would create a new task and title it thusly:

![Cookies Step 1][cookies_step_1]

I would then add the steps for collecting and combining ingredients and baking the cookies under this task.

![Cookies Step 2][cookies_step_2]

### Second, Configure labels and priority accordingly

Using multiple select, grab items and apply any additional information you need in the form of labels or priority. 

![Cookies Step 3][cookies_step_3]

#### Bonus Tip:

As you can infer from this image, I manage my grocery list as a filter on a specific set of labels for two big reasons:

* First, I can see *why* I'm buying something by looking at the project.
* Secondly I can arrange the filter to display the list in an order that matches my usual route through the different sections of my grocery store.

Keep in mind you'll need some additional method of keeping template items off your list filter, like filtering out items without dates and/or priority, or another label. Send a [tweet](https://twitter.com/sam_ferree) my way if you want to hear more about how I manage my grocery/shopping list with Todoist.

### Finally, Duplicate the task template, change the name and move to the correct project.

When I'm ready to use the template, I would select the options on the title task (Bake Cookies for) and select duplicate. I would rename the title task of this duplicate "Bake Cookies for The Big Game".

Then I would select the options on the title task again and move into a project, like "The Big Game Party"

![Cookies Step 4][cookies_step_4]

# Drawbacks of Task Templates

While the Task Templates offer several advantages over project templates, they have two major drawbacks as far as I can tell.

### No variable substitution

While this feature isn't available for project templates either, a true "template" would allow you to name it something like "Post {recipe} for Meal Monday" and then, in the process of using the template, define a value for {recipe}. 

### No relative date syntax.

Project templates still allow you to do relative dates, and while you *can* define dates in sub tasks relative to their parent tasks, they are expanded before being saved, so updating the date of the parent task, doesn't cascade down into updated dates for the sub-tasks.

[sub_tasks]: /assets/img/2018/1/31/sub_tasks.png "A Task with Sub Tasks" 
[section_header]: /assets/img/2018/1/31/section_header.png "Creating a section header"
[section_header_edit]: /assets/img/2018/1/31/section_header_edit.png "An example of a section header"
[multi_select]: /assets/img/2018/1/31/multi_select.png "Selecting more than one task for editing"
[duplicate]: /assets/img/2018/1/31/duplicate.png "Duplicating a task"
[cookies_step_1]: /assets/img/2018/1/31/cookies_step_1.png "A cookie example, creating the template"
[cookies_step_2]: /assets/img/2018/1/31/cookies_step_2.png "A cookie exmaple, adding sub-tasks"
[cookies_step_3]: /assets/img/2018/1/31/cookies_step_3.png "A cookie example, configuring steps"
[cookies_step_4]: /assets/img/2018/1/31/cookies_step_4.png "A cookie example, duplication and project placement"

