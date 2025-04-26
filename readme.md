This is an experiment. 

"What if we don't use react, tailwind, vite or next? What if we did Vanilla?"

The case is a CV builder. Desktop-only. No mobile.

We will do no backend and use localStorage for data.

> When you say "Everything will reside in one file" - do you mean one HTML file with embedded JS and CSS, or are we allowing separate files but just keeping them in the same directory?
Everything will reside in one HTML file as long as it's doable. 

> Are we using any build process at all, or is this purely serving static files?
We will use no build tool as the HTML file works as is out of the box. It will later be deployed on github pages.

> Are we targeting any specific browsers or versions?
We will use baseline as much as we can. Which means: Use old-school for everything, but if there is an API that really helps us, we will consider it, too.


> What fields/sections are we planning to include in the CV builder?
So far we will focus on the main points (personal, contact, summary, work experience, education, skills). In the future we might add.

> Are we planning to support multiple CV templates/layouts?
There will be a style "tab" where we set up a style. We might enable export import for that in the future but will not prepare that ahead. YAGNI.

> Are we planning to support multiple languages/i18n?
English only. We are a dev and we do it for ourselves and other devs or IT professionals. We assume they know the langua franca(not JS, but EN in this case ;).

> What's our strategy for localStorage? Single key for the entire CV or multiple keys for different sections?
Good question. Simple. Flat. An example. Job_<timestamp>: {company: <NAME>, start: <DATE>, end: <DATE>, title: <NAME>}

"Everything" will have: last_updated, since that can help users to know when they worked last on it. 

> Are we planning any data validation?
Basic for now. For example, dates will use the date input. But that's it. We are not concerned about security. Everything stays on users computers/browsers anyway.

> Should we implement any data backup/export features since we're using localStorage?
Yes, very probable, but we will not prepare it until we develop it.

> Do you want to set up any linting or code formatting rules?
Defaults are ok. Which means Cursor/VSCODE defaults for now.

> Are we implementing autosave? 
Maybe. We will not prepare but it's a good idea.

> Should we add form validation feedback? 
For now we will use "required".

> How should we handle larger images (like profile pictures) with localStorage limitations?
We don't. For now. And we will not prepare. But could be a cool future feature.

> Since we're working with a single HTML file, how do we want to handle development iterations? (e.g., commenting/uncommenting sections, versioning ).
Nothing will be "commented out". We work as a solo and will just save progress. Since we have instant feedback we are no longer concerned about the old problems like long compilation or anything like it. We just move fast.

> Do we want to establish any code organization patterns within the file? (e.g., keeping CSS at top, JS at bottom)
We will do locality-first. We will try to keep everything that is related to each other as close to each other. I hope you can already see the pattern in the file.

> How should we handle localStorage errors (e.g., quota exceeded, private browsing mode)?
We will adress it if it comes up. I don't think it's a big concern.

> Should we implement any error reporting for users?
We will try to not have errors and handle issues as gracefully as possible.

> Are we using any specific UI pattern for editing (inline editing vs. modal forms)?
That is an interesting question. UX is not my main skill. For now we will continue top down menu. We can move fast so we will redo it if it annoys us.

> Should we implement any undo/redo functionality?
No. The CVs will be the "versions". I have to rely on users to export data later and use git to version it.

> Do we want to show a preview of how the CV will look while editing?
Yes. On desktop I would like it to be visible all the time. On mobile a big switch button on every screen.

> Should we implement any data cleanup for old/unused entries?
No. Interesting idea though.

> Do we want to implement any versioning for the CV data?
Not for now and we will not prepare it. Also an intersting idea.

> Should we set any performance benchmarks since we're going vanilla?
Do you see an issue already? How?

> Do we want to implement any lazy loading patterns for potential future features?
Not now. If this is an issue, we will do a frame that loads quickly and to one to ten quick AJAXes or something to load in the rest. We will not prepare for this.

> Since we're going vanilla and using localStorage, should we add any console logging/debugging helpers for development?
That's a neat idea. Maybe later. If so: A console.groupCollapsed with the complete data maybe. Will not prepare for that.

> Would it be useful to have a way to clear/reset all data during development?
Not sure. I will keep it in mind, but this is so far the lowest priority.

> Are we using semantic HTML5 elements for better accessibility?
Yes. Let's be very semantic. 

> Should we establish any naming conventions for IDs and classes?
I like using window.elementsID instead of getElementByID. So no dashes. The case shoud be camelCase (?). Only use ids if we have to. Only use classes if we have to. We will mostly do inline CSS in elements and only do buttons at the start of the document in style tags.


> Abstractions? When do we abstract?
We avoid abstractions. Rule of three though. 



