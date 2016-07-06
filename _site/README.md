# Jekyll Resume Builder

This site started out with the idea of working out how to build a resume with Jekyll. Rather than Pages and Posts it makes use of Collections to populate the single page. 

## The Way it Works

All of the configuration take place in the _config.yml file.

### Site Settings

This set of values allows you to change the main settings heading and tagline of the site - plus set the baseurl (which you might need to change if you rename the directory of where the site is hosted)

### Collections Builder

This area sets up each of the collections currently included in the site. Each of the Outputs is set to false to stop Jekyll from unnecessarily generating additional HTML pages. 

### Colour Configuration

Allows you to set all the colours used throughout the site without having to get into the CSS file. 

### Folder Structure

Each folder in the site contains a markdown file for each section. For areas like Awards, Education, Experience, Interests, Publications and Skills you can add multiple files. You just need to use the same YAML structure as the dummy sections. 

The Profile section just has a single page. With the profiles listed you can remove or add them from the YAML front end, but you will also need to add/remove them from the index.html

## Customising

The Resume builder is completely customisable but you will have to do some editing. To create new sections - create new Collections in the config file, create new folders, and customise your YAML front end. 

The index file fairly clearly shows how to build a section. I've used IDs and Sections and then referred to them in the CSS (see bottom of the file) to create the alternative coloured sections. 

You can swap out the header image by changing the ```bgimage:``` in the config file. Centred images work best for the responsive design. 

## Pointing a URL 

This site works great running in GitHub Pages - basically giving you free hosting. You just need to change the branch to ```gh-pages``` and then add in a CNAME file with the domain to the root folder. [Instructions are available here](https://help.github.com/articles/using-a-custom-domain-with-github-pages/)