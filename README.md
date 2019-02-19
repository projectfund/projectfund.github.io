## Project Fund - A new delegate proposal

**INTRODUCTION**

Hello everybody!

As many of you know, my name is Dan (outboard). I've been an active member of the community for almost a year and have enjoyed watching ARK go through it's various phases of development and strife. From August 2018 to January 2019, I had the priviledge of serving as a board member of the [Ark Community Fund](https://arkcommunity.fund). Earlier this month (February 2019), the new board asked me to take on the role of advisory board member, a role which I happily accepted.

I'm a digital nomad, US citizen, and father of 2 who currently resides in Europe. My existing delegate, `arkoar.group`, has been actively forging since April of 2018 and is backed by my Estonian company, [Cryptobuilders OÜ](http://cryptobuilders.io). I hope to make this project the next phase of my involvement.

**THE PROPOSAL**

Recently, I've been greatly encouraged by the few delegates, including `jarunik` and `alessio` who have adopted models outside of the tradition profit share approach. I've also noticed that funding technical projects within the community has been a very adhoc effort. Many times, a small bit of funding is raised but the project stalls. You all know the ones I'm thinking of. Other times, a project takes ongoing effort and the pricetag raises great concern. My ACF board was part of making some serious waves when we approved a $30,000 rebuild of the core in Python. That project in particular made me realize that the ACF was not set up to fund ongoing development.

[Project Fund](http://projectfund.app) is here to facilitate community incubation of technical projects.

The delegate, when funded, will provide 0% profit share to it's voters. Instead, it's funds will be used to match community funding of tech projects. These projects must be built in some way on the ARK blockchain. [Project Fund](http://projectfund.app) itself will be build on top of ARK.

Anyone with an ARK wallet will be able to post a project for community funding. An admin team, consisting of volunteer community members with tech backgrounds will provisionally approve these projects for listing on the site. The criteria for approval is simple... build an app, tool, or open source library on ARK (new project or feature adds).

**THE PROCESS**

- A project is posted including a **description**, **minimum funding amount**, **desired funding amount** and **funding duration** *(ex. $1000, $2000, monthly)*
- An admin approves the project
- A unique ARK wallet is created and posted on the project's page
- The developer solicits donations from the community
- [Project Fund](http://projectfund.app) matches those donations 1 to 1 automatically

Once a project meets it's **minimum funding amount** *($1000 in our example)*, it is considered funded. A funded project's funds will be released, again automatically, after the **funding duration** has past *(one month from approval in our example)* or when the **desired funding amount** *($2000 in our example)* is acheived. As soon as the funds are released the funding duration begins again. On subsequent funding rounds, the funds are only released at the end of the **funding duration**, and only if the **minimum funding amount** is surpassed.

A project is considered to be over / archived when a single **funding duration** expires without successfully raising the **minimum funding amount**. When a project is archived, any unreleased funds are returned to the original donors.

Again, all of this happens automatically without the intervention of a board, elected or otherwise. The community votes with their wallet. Nothing more, nothing less. No further obligation.

**WHY?**

Tech projects aren't being built on mass around ARK. There is no incubator to speak of in the ecosystem beyond the team itself. Even work done on the core gets paid for after the effort is expended, discouraging anyone who doesn't have the free time to contribute. Conflict of interest rules around the ACF mean that 7 highly active members of the community are not eligible for any funding from the only community run funding entity. `Jarunik`'s efforts are great, but he can't be expected to do it alone.

**HOW THIS DIFFERS FROM THE ACF**

- **It's automatic** - There are no delays in funding. When a project hits the funding thresholds, it is funded
- **No COI** - Conflict of interest is not a thing because the community makes the choice as to which projects get funded, not the admins or operators of the delegate
- **Whale Resistant** - The board elections for ACF are a popularity contest decided primarily by whales. To have the same impact here, the whale would need to give away their funds.
- **No Funding Cliffs** - As a delegate, [Project Fund](https://projectfund.app) will have a steady stream of funding. Ongoing donations from the community are part of the design.
- **Legally Backed** - There is an actual company, registered in Estonia, backing the operation of this delegate and the system as a whole.
- **Software Only** - [Project Fund](https://projectfund.app) only funds software projects.

**TIMELINE**

Development work on the project will begin as soon as the delegate starts forging. I expect it to take 2 - 4 weeks to complete the initial buildout. There will be 2 applications required for the system to work.

- **A frontend One Page App** - Data will be stored on IPFS. The OPA itself will be a React frontend with no backend beyond IPFS and the ARK blockchain. Funding applications will be store on IPFS. The IPFS hash will be displayed to the applicant, who will then need to send it via smartbridge to the delegate wallet.
- **A backend listener** - A TypeScript listener app will listen for new funding application transactions to the delegate wallet and notify the admins via Discord. Once an admin sends a transaction to the delegate wallet approving the funding application, the listener will create a new ARK wallet to collect donations and a third transaction to the delegate wallet which will result in the "publishing" of the application on the frontend. The listener will then wait for donations to the project's wallet and send a matching donation from the delegate wallet automatically. Per the rules above, when the threshold for funding is met, the listener will send a "funded" transaction to the delegate wallet, updating the project's status and disburse the funds.

**FAILSAFE**

Admins will have the ability to manually archive any project the looks to be abusing the system. I will operate the delegate and assign admin priviledges. If it looks like anyone is attempting to game the system or is not doing anything to fulfill on their project, admins will archive their project before the next funding round. As long as the project owner is fulfilling on their self assigned goals, their project will never be manually archived.

If the delegate drops out of forging position, everything will continue to operate as normal until funds are exhausted, at which point matching donations will cease. Even if matching donations cease, [Project Fund](http://projectfund.app) will continue to operate as long as it receives enough donations from the community to pay for the backend listener's server and the transactions require to operate.

**REWARD SPLIT**

There will be no reward split. There will also be no COI provisions. Anyone, including me, will be free to create projects and seek funding. Voters should feel free to seek rewards in this way.

**MY SKILLS**

I have worked in IT as a Sysop, Software Engineer, Project Manager, Team Lead and CTO for 15 years. I am an expert in Ruby, Node / JavaScript / TypeScript, Elixir, and many other languages / disciplines.

**GOALS / ROADMAP**

The singular goal of [Project Fund](http://projectfund.app) is to encourage the development of real world services and applications powered by the ARK platform. Specifics of the matching algo may be tweaked, but all of the code will always be open source. We welcome contributions from the community as a whole.

**GITHUB**

- https://github.com/projectfund
- https://github.com/dmvt

**POTENTIAL PROJECT SUGGESTIONS**

- Core features
- Expansion to existing projects
- Plugins
- Wallet integrations
- dApps

**WHAT WE DO NOT FUND**

We will not approve any project that is not software development centric. There are many places, including the Team, ACF, and Jarunik, where a non-software project can get funding. We hope to fill a void in the current landscape of funding vehicles through this approach.

We will not fund anything deemed to be illegal in any jurisdiction where admins or the parent company [Cryptobuilders OÜ](http://cryptobuilders.io) operate. This is at my sole discretion as the owner of Cryptobuilders.

**THANK YOU**

To those who encouraged me to proceed with this proposal despite my doubts or desires to do it elsewhere, thank you.<br>
To those who back and vote for [Project Fund](http://projectfund.app)'s delegate, thank you.<br>
To voters of `arkoar.group`, thank you for sticking by me.

Dan
