# The Last Mile of Local-First
### Jess Martin
### May 28, 2025
---
# Hi!
### I'm Jess Martin.
### [jessmart.in](https://jessmart.in)
### [sociotechnica.org](https://sociotechnica.org)
 - Applied researcher 
    - bridging the gap from academic research to build real systems imbued with these qualities
- My focus is on the future of computing: enabling application interoperability
    - if you're interested in this, come find me

---
# Last Mile Problem

/assets/Clipboard 22.png
size: contain
- Last Mile Problems are famous in Telecom and Logistics
- Laid this complex network of infrastructure, and it's doing it's job of getting bits or packages around the world
- But the *last mile* to the customer's premises is the only way they *actually* benefit from this network!
    - You have to get to the customer's HOME or BUSINESS

---
# Local-first Software

## Croquet
## Fission
## Daylight Tablet
## DXOS

- Worked on several local-first frameworks and apps over the last few years
    - Croquet
    - Fission's WebNative / OddSDK
    - Daylight Tablet's sync system
    - DXOS
- Most recently, local-first landscape

---

/assets/Clipboard 4.png
background: true
y: top

### localfirst.fm/landscape
- My friend the esteemed Johannes Schickling and I created a resource called Local-first Landscape
    - it's a reference with all the different tools you could use to build a local-first applications.
    - I'm looking around the room and many of you have software that's listed there
    - breaks down all of the tools by capabilities so that you can quickly filter, sort, share, etc
- You should go check it out at https://localfirst.fm/landscape
    - Has a great mobile interface!
- 6-month deep dive into the local-first ecosystem
- In order to develop this resource, had to look at all of the systems that can be used to build local-first software and understand their capabilities
    - Worked on it for ~6 months
    - Reviewed dozens of systems
    - Talked to the creators of these systems
- I think that pretty well qualifies me to ... give a score to entire ecosystem

---
### A Local-first Scorecard
/assets/Clipboard 9.png
size: contain
	How are we doing as an _ecosystem?_

How are we doing at building software that conforms to the local-first ideals?
- If you've read the original Local-first Software paper (I won't ask for a show of hands) then you may remember this scorecard being applied to different software
    - Take the 7 ideals and turns them into three possible values:
        - CHECK for "yes!"
        - DASH for "sorta"
        - X for "nope"
- Rather than applying the score to a single ideal, I want to consider the ENTIRE ECOSYSTEM
    - How are we doing, collectiavely, at enabling software that maximally expresses the ideals?
- This isn't about a single piece of software or framework - I'm not here to crown any champions. It's about all of us.
---

	No spinners: 
	Multi-device:
	Network optional:
	Seamless collaboration: 
	Security and privacy by default:
	You retain ownership & control:
	The Long Now:

- Here's our scorecard.
- These are the 7 ideals from the original paper
- Six years since the article was published... we have solved many tech challenges!
- (and even longer since Offline-first and some of the precursor work)
- Let's take a look at how we're doing!

---

	No spinners: ？
	Multi-device:
	Network optional:
	Seamless collaboration: 
	Security and privacy by default:
	You retain ownership & control:
	The Long Now:

- First off: No Spinners
- Local-first software has gotten FAST!
    - not *all* software
    - Last year's conference was full of people talking about how fast their software is.
- Optimistic updates, etc
- Good work!
 
---

	No spinners: <span style="color:green; font: bold;">✓</span>
	Multi-device: ？
	Network optional: 
	Seamless collaboration: 
	Security and privacy by default:
	You retain ownership & control:
	The Long Now:
- Multi-device - how are we doing at getting data synchronized across multiple devices on different platforms?
- Sync engines are amazing!
    - Entire category devoted to solving this problem
    - It's almost table stakes for many application categories
- There's still hard work to do spanning the web and mobile, but we're working on it!
---

	No spinners: <span style="color:green; font: bold;">✓</span>
	Multi-device: <span style="color:green; font: bold;">✓</span>
	Network optional: ？
	Seamless collaboration: 
	Security and privacy by default:
	You retain ownership & control:
	The Long Now:
- Network optional
- Full offline support is possible!
- This is about more than just offline support:
    - Still need a server or at least a sync server
    - Still a lot of work to do to make P2P fully reliable and easy, but it's getting better
- Until we have full P2P over bluetooth or some ad-hoc local networking in our software, I don't think we can give ourselves a full green check here
- MINUS
---
	No spinners: <span style="color:green; font: bold;">✓</span>
	Multi-device: <span style="color:green; font: bold;">✓</span>
	Network optional: <span style="color:orange; font: bold;">–</span>
	Seamless collaboration: ？
	Security and privacy by default:
	You retain ownership & control:
	The Long Now:

- Lots of hard work on CRDTs and other methods of reconciliation
- There are still cases where it's hard, but again, it's so good, it has become table stakes
- We need to extend seamless collaboration beyond coding and design tools, but the path has been laid - it's _possible_
    - Props to Ink & Switch for Jacquard


---
	No spinners: <span style="color:green; font: bold;">✓</span>
	Multi-device: <span style="color:green; font: bold;">✓</span>
	Network optional: <span style="color:orange; font: bold;">–</span>
	Seamless collaboration: <span style="color:green; font: bold;">✓</span>
	Security and privacy by default: ？
	You retain ownership & control:
	The Long Now:

TODO: what to say?
- We're not quite there yet
    - See Brooklyn's talk
- Auth protocols still require a good deal of centralization and server authority.


---
	No spinners: <span style="color:green; font: bold;">✓</span>
	Multi-device: <span style="color:green; font: bold;">✓</span>
	Network optional: <span style="color:orange; font: bold;">–</span>
	Seamless collaboration: <span style="color:green; font: bold;">✓</span>
	Security and privacy by default: <span style="color:orange; font: bold;">–</span>
	You retain ownership & control: ？
	The Long Now: ？

What about these last two?
What did the original authors mean by these?
Let's ponder


---
### Ownership and control is about _Agency_.

	> "we mean ownership in the sense of **user agency, autonomy, and control over data.** You should be able to **copy and modify data in any way**, write down any thought, and **no company should restrict what you are allowed to do.**"

> does not mean that the software must necessarily be open source. [...] it is possible for commercial and closed-source software to satisfy the local-first ideals, as long as it **does not artificially restrict what users can do with their files.**


- Giving users the ability to copy, modify, tweak, repurpose, integrate, remix their data
- No company should restrict users ability to *work with* their data
- Doesn't imply access to the software's source - so long as the software doesn't restrict user's capabilities


---
### The Long Now is about _Agency, forever_.

	> "When you do some work with local-first software, your work should **continue to be accessible indefinitely**, even after the company that produced the software is gone."

> **Some file formats (such as plain text, JPEG, and PDF) are so ubiquitous** that they will probably be readable for centuries to come.

> However, in order to read less common file formats and to preserve interactivity, you need to be able to run the original software (if necessary, in a virtual machine or emulator).


 
- Access your data in the future - not just about "on my hard drive"
- File formats that are guaranteed to be accessible
    - I still have some documents written in Claris Works
        - anyone? hands?
    - I can't open those anymore with an emulator - there is _no software_ for opening ClarisWorks files on modern computers
    - I have the files! the format is dead.


---
/assets/Clipboard 16.png
size: contain
- Let's look at a typical local-first architecture
- Generically, it looks something like this:
    - Multiple devices
    - Sync data between those devices via a sync server or centralized server
    - Store the data in local data stores on device
- We're getting the data to the user's devices.
- But it's still _trapped_ inside the applications' datastores.
- No way for a user to access their own data when it's stored in the browser's file system or a sqlite db


--- 
	No spinners: <span style="color:green; font: bold;">✓</span>
	Multi-device: <span style="color:green; font: bold;">✓</span>
	Network optional: <span style="color:orange; font: bold;">–</span>
	Seamless collaboration: <span style="color:green; font: bold;">✓</span>
	Security and privacy by default: <span style="color:orange; font: bold;">–</span>
	You retain ownership & control: <span style="color:red; font: bold;">Ｘ</span>
	The Long Now: <span style="color:red; font: bold;">Ｘ</span>
- I have to give all of us an X on user ownership and control and the long now
- It's not clear to me that users have any more agency over their data than they did five years ago 
- or that our software is going to last any longer than it did

---
### Local-First's "Last Mile"
/assets/Clipboard 14.png
size: contain
The Long Now and user-owned data are the _last miles_ of local-first software.

- Similarly, We're getting the data onto the end-user's device, but not onto their "premises." 
    - They don't have the data somewhere they can **control.**
- Just because data is actually on the user's device doesn't mean they can copy, modify, tweak, repurpose, integrate, remix
- Especially if the data stays trapped in proprietary, undocumented formats
PAUSE: RAISE YOUR HAND IF YOU ARE AN APP DEVELOPER.

---
### App Developers!
# The Last Mile is _your_ problem!
This is not a framework problem, but primarily a problem for App Developers to solve
- The last five years of advances have largely been solved by frameworks and libraries and a few intrepid software companies
    - Pioneering, hard work!
    - We got a lot of green checks on the scorecard! Good work!
- The "Last Mile" of local-first will have to be solved by application developers.
- In this talk, I want to issue a challenge to app developers.
- I'm going to provide a few levels to grade yourself on the support you provide to your users.

---
### Levels of Agency 
	### 1. Export to common formats
	### 2. Continuous export
	### 3. Bi-directional sync

Three levels to self-assess user agency in your software:
- Level 1: Export to common formats
- Level 2: Continuous export
- Level 3: Bi-directional sync

- Progressive enhancement, upgrading the user's agency within your software
---
### LEVEL 1
# Export to common formats
- Level 1 should be trivial - many of you already support this.
    - should be table stakes!
- Export allows the user to get the data on their premise
---
/assets/Clipboard 17.png
size: contain
- Unfortunately, this isn't really all the way to their premises yet
    - It's like putting a box outside their house with the data in it
    - They can go outside and fetch it
- This has to be initiated by the user each time
- But it's a start!
---
### LEVEL 1
# Export to _common formats_
- So many to choose from: Markdown, CSV, PDF, etc
    - No, "JSON" is not a common format!
        - it's a container
        - without documentation, JSON isn't much better than binary
- Choose one that's appropriate to your app's use case and user workflows
    - Think about the other applications that they work with
---
/assets/Clipboard 10.png
size: contain
/assets/Clipboard 11.png
size: contain

/assets/Clipboard 13.png
size: contain
- Why common formats?
- Common formats are an integration point
- N^2 to 2N
- Consider an application that has to integrate with another application
- Now let's add a third application
- At 5 applications we are already at 20 connections `(n * (n - 1))`
- Common format means we have 5 connections again
---
### LEVEL 1
# If it doesn't exist: invent and document
What if one doesn't exist? invent and document
---
	&nbsp;
/assets/xkcd927.png
size: contain
xkcd 927 doesn't let you off the hook

---
/assets/Clipboard 1.png
y: top

- Obsidian is well-known for their "File over App" philosophy
- They released a whiteboard, but needed a way to represent that as a file
- Designed and released JSON Canvas
    - Documented the file format for others to implement
    - Kinopio, a similarly simple whiteboard app, implemented it just a few days after Obsidian
 
---
### LEVEL 2
# Continuous export

- Think of this as a continuous projection of the app's data to an external source
    - Every write in the app causes a re-render of the projection
- Doesn't handle reads - just overwrites
- In our analogy, this is like running a read line to the end user's premises, but there's still no "write" line 
    - But it's really on their system!
- We already mentioned Obsidian
---
### Continuous export
/assets/Clipboard 18.png
size: contain
---
# Demo time
/assets/Vintage Electronic Project Kit Display.png
background: true
y: top
opacity: 40%
- Kanban.md demo
---
### LEVEL 2
# Doesn't have to be files!
---
/assets/linear-to-google-sheets.mp4
size: contain
Linear -> Google Sheets DEMO
- Doesn't have to be files!
- Linear → Google Sheets DEMO
- Build charts, run calculations, etc
--- 
### LEVEL 3
# Bi-directional sync
---
### LEVEL 3
# Continuous export
### *and*
# update from external source
---
/assets/Clipboard 19.png
size: contain
- Running the read *and* write lines to the end user's premises!
    - They can write to the file as well
---
# Demo time
/assets/Vintage Electronic Project Kit Display.png
background: true
y: top
opacity: 40%
- Obsidian implements this via the file system 
- Kanban.md can write, too!
    - So satisfying to drag a card over!
--- 
### LEVEL 3
# Welcome to hard mode
	Seph? Rasmus? #plsfix
- Back in the land of open research problems...
- Much harder!
- But now we are back in the land of open research problems
    - Substrate matters...
        - File system? CLI agent? Desktop app?
        - Playbit, Seph Gentle's OS
    - Particularly challenging for real-time collaboration, as changes aren't automatically available as "diffs" or "patches"
        - And merging of offline edits
- But amazing things are possible if you do the work...
---
# Demo time
/assets/Vintage Electronic Project Kit Display.png
background: true
y: top
opacity: 40%
- Show a Obsidian Canvas ⟷ TLDraw demo powered by OCIF
- TLDraw: Add a Rectangle on the left
- TLDraw: Copy the Rectangle to the right
- Obsidian: Change the label for the Rectangle
- TLDraw: Draw an arrow between them
- TLDraw: Drag the rectangles
- Obsidian: Drag the rectangle on the left
    - This is slow, because of file system limitations
- Collaborate _across_ applications!
    - Application interoperability!
    - THE DREAM!!
---

### WUT?
/assets/Clipboard 20.png
background: true
x: left
- How does this work?
- JSON Canvas from Obsidian is a format
- Did TLDraw add support for JSON Canvas?
- Nope.
---
/assets/Clipboard 25.png
size: contain
y: top
- March 2024, Orion Reed and I were each working on file formats for infinite canvases when JSON Canvas was released. 
- Unfortunately, JSON Canvas is too simple and non-extensible
- Orion tweeted about starting a working group to pioneer an open canvas format
- I said sure!
- Open Canvas Working Group was born!
---
/assets/JPEG image-495A-ADFF-1A-0.jpeg
background: true
- Last year at Local-first Conf, Orion and I wrote the first draft of the spec which became OCIF

---
/assets/Clipboard 21.png
size: contain
- The Open Canvas Working Group met 25 times over the past year
    - Git issues
    - Input from 15 canvases
    - Multiple spec versions
    - 3 canvas implementations
    - Several new collaborators
- There's a solid spec
---
/assets/Clipboard 26.png
size: contain
- So how did that demo work?
- TLDraw <> OCIF
    - via websockets
- JSONCanvas <> OCIF
    - via the file system
- The real magic is OCIF itself
    - Convert both to/from OCIF rather than directly to each other
---
### Humans aren't the only readers.
# LLMs understand open formats.
- Humans aren't the only consumers
- Because there's a well-documented spec, AI are quite good at generating OCIF from a text description 
- And understanding an OCIF file based on a description

---
# Demo time
/assets/Vintage Electronic Project Kit Display.png
background: true
y: top
opacity: 40%
- A few quick demos of AI working with OCIF
    - AI explaining a canvas
    - AI writing a canvas based on a prompt, etc...

> Create a diagram of the branches of the United States government, the title of the elected officials in charge of each branch, and their relationship to each other. 
---
### OCIF is at
# Candidate Recommendation
	Come kick the tires!
- As of today, OCIF is at Candidate Recommendation
- We are _roughly_ following the W3C process
- Candidate Recommendation means:
    - We feel the spec captures the majority of cases and is relatively complete and stable
    - And now it's ready to be implemented
        - Two app that have implemented already and we have a handful of demos
    - _But_ the spec will still change as we seek to incorporate feedback from implementers
        - Feel really good about the spec
- If you are working on a canvas, consider implementing import/export OCIF
    - You can implement in our "tools" package which will give users access
    - Through the CLI tool
    - And through the exporter website

---

### App devs 
	Take us the Last Mile:
	- Export common formats.
	- Continuously export.
	- Explore bi-directional sync.

### Canvas devs
	Try out OCIF:
	canvasprotocol.org

/assets/Clipboard 23.png
size: contain



- Show score card again
- Give users control and solve for the Long Now!
- Reiterate Last mile story - show the phone lines again
