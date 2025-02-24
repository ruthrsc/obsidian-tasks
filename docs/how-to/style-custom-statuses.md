---
layout: default
title: Style custom statuses
nav_order: 3
parent: How Tos
---

# Style custom statuses
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---

## Motivation and assumptions

After setting up [setting up our custom statuses]({{ site.baseurl }}{% link how-to/set-up-custom-statuses.md %}), they look very unappealing in Obsidian.

This pages walks through downloading and using a CSS snippet to make them look good.

We assume that you know how to [use CSS snippets in Obsidian](https://help.obsidian.md/How+to/Add+custom+styles#Use+Themes+and+or+CSS+snippets).

## Summary

If you are using custom statuses in Tasks, you will need to install and enable **one of** the following, in order for your tasks to look good:

- A custom CSS Snippet
- A Theme

We recommend selecting a snippet rather than a theme.

This is because if you choose custom checkboxes from a theme, you are tied that theme permanently.

However, most snippets can be applied to any theme, giving you much more flexibility.

## Default appearance

Suppose we had these three tasks with custom statuses:

```text
- [!] #task Do important stuff
- [D] #task Do important stuff
- [X] #task Do important stuff ✅ 2023-01-09
```

Tasks doesn't know the meaning of any custom statuses. This means that by default, these tasks would be displayed like this:

![Default appearance of 3 sample tasks](../images/styling-sample-tasks-default-appearance.png)

- We intended the first two tasks to be 'not done', but they have a checkmark.
- All three tasks look like they are done, because none of them has a space in the `[]`.
- Only the one with `[X]` has a line through it. Tasks only treats lines with `[x]` or `[X]` as completed.

## Picking a custom style: SlrVb's Alternate-Checkboxes

There are many community Snippets and Themes available to customise the appearance of checkboxes in Obsidian, and different people have different preferences.

Tasks allows (and requires) you to choose your own styling option.

For this example, we will choose to style our tasks with SlrVb's [Alternate-Checkboxes](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Guide/Alternate-Checkboxes.md) from the [ITS-Theme.](https://github.com/SlRvb/Obsidian--ITS-Theme).

Download the snippet, add it to your vault's snippet folder, and enable the snippet.

The above 3  task lines now look like this:

![3 sample tasks styled with SlrVb's Alternate-Checkboxes](../images/styling-sample-tasks-slrvb-custom-checkboxes.png)

### Customising the custom style: Style Settings plugin

We also have the option to install the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin and customise the appearance of SlrVb's Alternate Checkboxes.

- Use this link to [install the Style Settings plugin in your vault](obsidian://show-plugin?id=obsidian-style-settings)
- Enable the plugin

Now we can go to the Style Settings plugin's options:

![Initial appearance of Style Settings plugin options](../images/styling-sample-tasks-style-settings-options-1.png)

Expand the 'SlRvb's Checkboxes' section and turn on these options:

![Style Settings plugin options after making a few changes](../images/styling-sample-tasks-style-settings-options-2.png)

Now the above three tasks look more colourful, and tasks with `[x]` and `[X]` are crossed out, indicating they are completed:

![3 sample tasks, with SlrVb's Alternate-Checkboxes modified by Style Settings](../images/styling-sample-tasks-slrvb-custom-checkboxes-modified.png)
