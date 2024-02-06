<h1 align="center">Task Management </h1>




Track tasks across your entire vault. Query them and mark them as done wherever you want. Supports due dates, recurring tasks (repetition), done dates, sub-set of checklist items, and filtering.

_You can toggle the task status in any view or query and it will update the source file._

---

## Screenshots

- _All screenshots 

![ACME Tasks](1.png)


![Important Project Tasks](2.png)


![Tasks Queries](3.png)


![Create or Edit Modal](4.png)
![Create or Edit Modal](5.png)
![Create or Edit Modal](6.png)
![Create or Edit Modal](7.png)



## Installation

Follow the steps below to install Tasks.

1. Search for "Tasks" in Obsidian's community plugins browser
2. Enable the plugin in your Obsidian settings (find "Tasks" under "Community plugins").
3. Check the settings. It makes sense to set the global filter early on (if you want one).
4. Replace the "Toggle checkbox status" hotkey with "Tasks: Toggle Done".
    - I recommend you remove the original toggle hotkey and set the "Tasks" toggle to `Ctrl + Enter` (or `Cmd + Enter` on a mac).

## Getting Started

### Write some tasks

Create a few tasks in a Markdown note in your vault. For example:

```text
- [ ] Something non-important, with no date
- [ ] Remember to do that important thing - with a due date 📅 2022-12-17
- [ ] Send Kate a birthday card - with a scheduled date 🔁 every January on the 4th ⏳ 2023-01-04
```



### Create your first Tasks search

And then write a Tasks search block somewhere in your Obsidian vault, to find the tasks that are interesting.

Here is an example that shows a few different features. View it in Reading or Live Preview modes to see the results.

````text
```tasks
# Only tasks that are not done, that is, which begin like this (but without the quotes):
#   '- [ ] ' or
#   '* [ ] ' or
#   '1. [ ] '
# Indented tasks are supported, but only single-line tasks.
not done

# Tasks due today or earlier:
due before tomorrow

# Restrict to at most 100 tasks.
# If you ask Tasks to display many hundreds or thousands of tasks,
# Obsidian's editing performance really slows down.
limit 100

# Group and sort the output:
group by filename
sort by due reverse
sort by description

# Optionally, ask Tasks to explain how it interpreted this query:
explain
```
````


