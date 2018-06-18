# WDTK
The (Freelance?) Web Developer's Tool Kit (WDTK). A flexible bundle of tools and services for web developers with many projects, or many clients.

This project is just an idea at the moment. It's been floating around my head for the past couple of weeks, I'm trying to validate the idea by asking other devs what they think. If you have an idea/critisism/request open an issue and let me know.

## What's the Big Idea?

I'm a freelance web developer, over the years I've picked up lots of clients and worked on lots of projects. I'd like a way to manage my past, present, and future projects. Here's a rough timeline for a project:

**1. Start Relationship with Client**
Start talking, exchange some emails, have phone calls, or other online chats. Scope out the project, the requirements, deadlines, and priorities. Talk about money. Sign contracts, or NDAs.

**2. Start Work**
Build things, share works in progress, get feedback. Re-prioritise things, learn what the client actually wanted to build. Re-build things, iterate and improve.

**3. Sign Off and Complete**
Finish all tasks, client is happy. Hand over code? Help host in production? Deal with DNS, SSL, email, backups, etc. etc. Get paid!

**4. Archive and Monitor**
Work is finished so archive code, shut down demo sites, wash hands. Set up monitoring so if things go wrong, you know about it. Mostly forget everything about this project.

There are lots of things here, freelancing can be complicated. Especially when you factor in the number of projects you work on over the years, and how few projects end up sharing solutions and services. One client already uses AWS, one likes DigitalOcean, nobody shares the same domain registrar.

I'd like a single toolkit where I can keep all of these things. A website I can use to manage my projects, through all 4 steps. Here are some features I'd like to see:

- File storage (for uploading contracts, or keeping static assets)
- Task management (issue boards, kanban, todo lists, etc.)
- Invoicing? (Not sure about this one, maybe out of scope)
- Version control
- Online chat, or some kind of communication service
- Demo site hosting
- Automatic backups of everything
- DNS monitor
- Uptime monitor
- Dead link checker, or some kind of web scraper
- Easy archive options
- Everything encrypted
- User accounts that can be created for clients (so with limited access)
- Open source, with an active community

The thing is, this needs to be incredibly flexible to deal with how varied each project can be. One demo site might use SQLite3, the next might use MongoDB. One client wants to use Trello for tasks, the next, JIRA.

So how about a website that managed Docker containers in a simple way. Want to spin up GitLab? Use a GitLab image. Need Ruby on Rails with PostgreSQL? Go for it.

It also needs to be able to link out to external services where used, e.g. Trello, or AWS. Maybe with notes on how they're used.

## Similar Ideas (and Why I Don't Think They Fit)

**Sandstorm**
Runs apps on your own server so probably meets most requirements. I think that it doesn't support Docker, so I'm uncertain how easy it would be to package up lots of custom apps (e.g. for demo sites). Also, it's pretty ugly, and I wouldn't really want to share it with clients.

**Cauldron**
Runs apps on your own server, so probably meets most requirements. Looks like it supports Docker fairly well. It's not free, and limits are quite strict for the kind of uses I had in mind (e.g. open app lots to start with, then very rarely). Some of it is open source (I think??) so could use this as a base?

**Flockport**
Similar to Cauldron, more focus on docker. Looks like it's free but not open source? Might be worth keeping an eye on.

**Libre.sh**
Very Docker focuessed and definately open source. Doesn't come with a web interface, so there might be some more work required to get it to where we need.

**Bitnami**
Can't get a good read on what this does. I think it's a bit more like an enterprise solution for production applications. So maybe not a good fit for this?
