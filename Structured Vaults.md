## Structured Vaults

![[ill_blog_hero_img_Inside_Man_1450x625.jpg]]

---

### A Personal Wiki

Obsidian is essentially a personal Wiki with automagical rendering built-in, as well as some really great additional features.

This provides a lot of flexibility in how you decide to use it.

---

### Some considerations

- How do you think about your notes?
- How do you like to interact with your notes?
- How do you best think about what goes into a vault?

---

### One Vault to Rule Them All

You may decide to only use one vault for everything, which comes with certain advantages - for example, all of your data is now interconnect(ed/able).

A benefit of this is that you can find surprising, new connections between discrete bits of data.

---

### Context Vaults

Another strategy is to use vaults as a kind of box to separate different categories of information.

I would call these _'context aware'_ because everything in the vault is valid in the context of that vault.

---

An example from how I use vaults:
- CV
- Freediving
- Language Learning
- TIL
- Engineering

---

Each vault contains information relavant to a specific context. I use the vault to create boundaries between data, so that data does not _leak_ between contexts.

---

The reason for this is simple - I want to create a rich and interconnected web of information _within the context of a vault._

This is an engineering concept.

---

Partitioning my data like this has the advatage that there are never gaps in knowledge, and if I find that I have large, discrete chunks of data in a vault then I split them into two vaults.

---

Since all data is stored as local text files, I can _always_ build a **"master vault"** with all of my data if I need to.

I would simply copy everything into a single folder. 

---

Combining data is trivial. 

Separating data is difficult. 

---

Start by separating your knowledge into contexts, then mix and add salt to flavor. 

---

### Why do this?

- Suppose I am considering writing a book on a specific topic. I can now use my vault to enforce the boundaries of that context.

- I use vaults as a __clear mode__ for how I interact with my knowledge - I do not hold the same space and intent when taking notes from a talk by Samuel as I do when I am pulling research from the internet.

---

### Un-Conventional

How you structure your vaults _(or don't!)_ is up to you - Obsidian is convention-agnostic.

---

### My Basic Vault Structure

- Top level folders to represent a knowledge context
- Use sub-folders to keep the contexts clean
- If 3-deep folders, ask if there is a way to split the context

---

### Vault Structure

- `_` delimited folders are data-related
- `_media/` is for all media
- `_media/_images/` contains all images
- `_templates/` contains all template files
- all template files are named `something.template` so that I never make a mistake.

---

### Exercise: Create a context aware vault

Take a 5 minutes to create a new vault for some topic that you are interested in.

Setup a basic vault structure, thinking about how your data could be separated into contexts. Create the following folders:
- `_media/`
- `_media/_images/`
-  `_templates/`
 
---
 
### Templates

A super convenient way to layout the style of a note in advance.

A template is a note that will be used to generate new notes.

---

### Exercise: Your first template

- Settings -> Core Plugins -> Templates -> Turn it on
- Settings -> Options -> Templates -> `_templates` as your folder location

--- 

### Exercise: Your first template

- `ctrl + n` -> New Note -> Title -> _page.template_
	- Body ->
		```
		# {{ title }}
		
		## Notes
		```
- Right click note -> Move file to... -> `_templates/`

---

Now that we've created a template, let's see what it does...

---

### Exercise: Using your template

- `ctrl + n` -> New Note -> Title -> _Whatever you want_
- Ribbon icon (bottom icon on the top right stack) -> Insert Template ->  `_templates/page.template`

---

You should now see your title displayed in as an `h1`,

```
# Whatever

## Notes
```

---

### Kittens!

![[kitten.jpeg]]

---

### Exercise: Images

Having a `_media/` folder allows us to easily manage data in a template.

In your new note, add an image and then move it to the `_media/_images/` folder.

---

### Embedding Videos

The ability to embed videos with an `<iframe>` is a killer feature.

<iframe src="https://www.youtube.com/embed/BeL5dI5Hkg8" />

---

To do this, we use an `<iframe>` tag like so,

```
<iframe src="https://www.youtube.com/embed/BeL5dI5Hkg8" />

```

Where the url is `https://www.youtube.com/embed/{VIDEO_ID}` and `{VIDEO_ID}` is what you find at the end of a Youtube video url.

---

### Exercise: Embed a video

Give it a shot. Right now.

```
<iframe src="https://www.youtube.com/embed/BeL5dI5Hkg8" />

```

---

### What is an iframe?

An iframe is an html tag that allows us to embed an html document inside another html document.

What we just did is embeded an html document containing only a video inside our iframe. 

But we could do so much more...

---

### Can we embed a whole website?

---

### The Clove Hitch

Yes we can,

<iframe src="https://www.animatedknots.com/clove-hitch-knot-rope-end" height="500"/>

---

```
<iframe 
src="https://www.animatedknots.com/clove-hitch-knot-rope-end" 
height="600"/>
```

_This is not semantic html - I needed to make it fit. You will never have a new line in an html tag._

---

### Exercise: Embed a website in an iframe

Use any url,

```
<iframe src="https://clairvision.org" />
```

---

Hopefully this will give you a starting point for getting into Obsidian and get your creativity flowing.

As they say...

---

![[biggie-smalls-cat.jpeg]]
> "Sky's the limit"
> \- _Biggie Smalls_
