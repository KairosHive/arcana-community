# Arcana community

[Arcana](https://arcana.kairos-hive.org) searches, maps and makes new work from
archives of photographs, sounds and videos, on your own computer. This is where
the people who use it show what they make, suggest what comes next and help one
another.

## Take part

| | Where | What to post |
|---|---|---|
| **Show your work** | [Show and tell](https://github.com/KairosHive/arcana-community/discussions/categories/show-and-tell) | boards, pictures, films and stories made with Arcana, and how you made them |
| **Suggest a feature** | [Ideas](https://github.com/KairosHive/arcana-community/discussions/categories/ideas) | what you wish Arcana did, and the work it would help with |
| **Vote on ideas** | [Ideas, most voted](https://github.com/KairosHive/arcana-community/discussions/categories/ideas?discussions_q=category%3AIdeas+sort%3Atop) | an upvote on the ideas you want most |
| **Ask a question** | [Q&A](https://github.com/KairosHive/arcana-community/discussions/categories/q-a) | how to do something, or why something behaves as it does |
| **Report a bug** | [Issues](https://github.com/KairosHive/arcana-community/issues/new/choose) | what you did, what happened, and Arcana's version |

The most voted ideas shape what Kairos Hive builds next. Announcements carry
each release and what changed.

Posting needs a free GitHub account. The **Community** menu in Arcana's header
opens each of these pages.

## Made with Arcana

Work shared in Show and tell can appear on the
[community page](https://arcana.kairos-hive.org/community) of the Arcana website,
with your name and a link to your post. A box in the Show and tell form asks for
your permission, and only posts with that box ticked are shown.

## The agent plugin

The [plugin](plugin/) connects Claude Code to the Arcana installed on your
computer and adds Arcana's skills, **moodboard**, **board-design**, **harmonize**
and **metaphysical-moodboard**. In Claude Code, run

```
/plugin marketplace add KairosHive/arcana-community
/plugin install arcana@arcana
```

The plugin starts `%LOCALAPPDATA%\Programs\Arcana\Arcana.exe`, where the
installer puts Arcana. The [guide](https://arcana.kairos-hive.org/guide#7-work-with-an-agent)
explains what to ask an agent. Skills you write yourself are welcome in Show and
tell.

## Guides

- [The workflow and every feature](https://arcana.kairos-hive.org/guide), on the website.
- [Intentional camera movement](docs/ICM_GUIDE.md), every ICM technique in detail.

## What you share

- Your work stays yours. Posting it here lets people see it on GitHub, and the
  ticked box lets Kairos Hive show it on the Arcana website with credit.
- Ideas and feedback may be built into Arcana freely, without payment or
  credit owed. The Arcana licence agreement says the same.
- Kindness and specifics help most. Describe the work, the archive and the step
  where Arcana helped or got in the way.

Arcana itself is closed source, copyright Kairos Hive. The plugin and its skills
in this repository are under the [MIT licence](plugin/LICENSE), so you can adapt
them.
