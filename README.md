# final_418

## AI Disclosure Statement

I did not use generative AI tools for this project. I used only approved course materials, instructor examples, documentation, and my own work.

## Development Log 
### Day 1 
- Started with GIT 417 final project as a baseline
- Installed jQuery
- Landed on toastr for my jQuery widget/plugin, installed and tested
- Started localStorage persisting cart contents, switching from previous system

## Debugging Log
### Problem 1 
The toastr popup did not appear.
### What I tried 
Checked my installation of jquery and popup.
### What fixed it 
Realized that I forgot to include links to the js files in the HTML (and to the toastr css)
### What I learned 
(Relearned :P) After installing with npm, don't forget to actually connect what you downloaded to your project.

### Problem 2
None of the add/remove buttons worked.
### What I tried 
This wasn't hard to find the root issue of, there's not a lot of code in here to debug.
### What fixed it
When implemented localStorage, I did not have a case to set the cartItem container to an empty object if the storage key was not present yet.
### What I learned 
Make sure that logic is built in around not finding appropriate storage keys.

### Problem 3
Slick (carousel) was causing errors and not functioning.
### What I tried 
It sounded like it might have been an issue reported on the site. I wasn't sure if it was the same problem, and the solution propose did not help. I tried moving my javascript file to load after the others as a sanity check.
### What fixed it
This is an old plugin, and sure enough reverting to an earlier jQuery version solved it.
### What I learned 
Verify the versions that your 3rd party resources use before going in to your project (make sure everything can use the same jQuery version in this instance)