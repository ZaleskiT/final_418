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