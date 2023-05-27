---
title: Version Control System. Git.

# Summary for listings and search engines
summary: Git is a good intrument for version control.
# Link this post with a project
projects: []

# Date published
date: '2023-03-17T00:00:00Z'

# Date updated
lastmod: '2023-03-17T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - Git

categories:
  - Education
---


## Overview


What is a "version control system" and why is it important? A version control system is a system that records changes to a file or set of files over time and allows you to return later to a specific version. For file version control, this book will use the source code of the software as an example, although in fact you can use version control for almost any type of file.

If you are a graphic or web designer and want to save every version of an image or layout (most likely you will), a version control system (hereinafter referred to as VCS) is just what you need. It allows you to return files to the state they were in before the changes, return the project to its original state, see the changes, see who last changed something and caused the problem, who set the task and when, and much more. Using VCS also means in general that if you have broken something or lost files, you can safely fix everything. In addition to everything, you will get it all without any extra effort.
Many people use copying files to a separate directory as a version control method (perhaps even a directory with a time stamp, if they are smart enough). This approach is very common because of its simplicity, but it is incredibly prone to errors. You can easily forget which directory you are in and accidentally change the wrong file or copy the wrong files that you wanted.
In order to solve this problem, programmers have long ago developed local VCS with a simple database that stores records of all changes in files, thereby monitoring revisions.
One of the most popular VCS was the RCS system, which is still distributed with many computers today. RCS stores on disk sets of patches (differences between files) in a special format, using which it can recreate the state of each file at a given time.
The next major problem that people face is the need to interact with other developers. In order to deal with it, centralized Version Control Systems (hereinafter CVCS) were developed. Systems such as CVS, Subversion, and Perforce use a single server containing all versions of files, and a number of clients that receive files from this centralized repository. The use of CVCS has been the standard for many years.


This approach has many advantages, especially over local VCS. For example, all project developers know to a certain extent what each of them is doing. Administrators have full control over who can do what, and it is much easier to administer CVCS than to operate local databases on each client.

Despite this, this approach also has serious disadvantages. The most obvious disadvantage is a single point of failure represented by a centralized server. If this server goes down for an hour, then during this time no one will be able to use version control to save the changes they are working on, and no one will be able to share these changes with other developers. If the hard disk on which the central database is stored is damaged, and there are no timely backups, you will lose everything — the entire history of the project, not counting single repository snapshots that have been saved on local developer machines. Local VCS suffer from the same problem: when the entire project history is stored in one place, you risk losing everything.
This is where Distributed Version Control Systems (hereinafter DVCS) come into play. In DVCS (such as Git, Mercurial, Bazaar, or Darcs), clients don't just download a snapshot of all files (the state of files at a certain point in time) — they completely copy the repository. In this case, if one of the servers through which the developers exchanged data dies, any client repository can be copied to another server to continue working. Each copy of the repository is a complete backup of all data.



