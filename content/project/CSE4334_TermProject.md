+++
date = 2019-01-28
title = "CSE 4334 Term Project"
+++

The most compelling reason why people would want this app is new and old experiences.  By having an easy method to find similar music they can expand their horizon finding more music they enjoy, or find old music they enjoyed but forgot the name.  This will also allow them to explore new types of music by seeing what is popular and recommended in a different genre.  As music has a large impact on people's emotions, this will allow them to find music for all moods.  This app is particularly useful as it displays the types of music based on the genres and the total number of people that follow the artists of that genre which cuts out some of the bias that big apps have toward mainstream artists.  In the end, this app will allow users to explore and find music in an easy and convenient manner.

{{% staticref "files/ProjectIdea.pdf" "newtab" %}}View the Project Proposal{{% /staticref %}}<br />
{{% staticref "files/usage scenario.pdf" "newtab" %}}View some Usage Scenarios{{% /staticref %}}<br />
{{% staticref "https://github.com/d2adams/CSE4334TermProject" "newtab" %}}View source code{{% /staticref %}}<br />
{{% staticref "https://youtu.be/Max6i3gqoMk" "newtab" %}}View Project Video{{% /staticref %}}

{{< figure library="1" src="AppUser.png" title="User Page Sketch" >}}
{{< figure library="1" src="AppSearch.png" title="Search Page Sketch" >}}
{{< figure library="1" src="AppArtist.png" title="Artist Page Sketch" >}}
{{< figure library="1" src="userPage.png" title="User Page Design Sketch" >}}
{{< figure library="1" src="searchPage.png" title="Search Page Design Sketch" >}}
{{< figure library="1" src="artistPage.png" title="Artist Page Design Sketch" >}}

Phase I:

The first phase of the development is to implement the search feature using support vector machine.  I used the dataset from lastfm that contains various artists, their tagged genres, and the number of users that have them tagged.  For this project I am creating a Android phone app that has the functionality hosted on a flask server via pythonanywhere.

During this phase of the project I was having problems with the search taking too much time to find results, and that the app would crash while trying to get the search results.  I am currently looking for methods that would make run time for the search more efficient, so that I can implement them for the later phases.  The problem with the app crashing was that the write could not complete without blocking. I was able to temporarily stop the problem by reducing the size of the dataset; however, that is not a permanent solution and I am looking into a way to fix it.

Phase II:

For the second phase of development I was able to find some methods that could reduce the time for searches by storing some of the values on the server itself.  The primary part of this phase is implementing a text classifier to find the genre based on user input.  I have currently been trying to implement either Naives Bayes or k-nearest neighbors, and see which one has the best results.

I am still having some issues with proper classification which might be due to the dataset or the algorithm not being properly written. Also, depending on the changes I make to the code, the app starts to crash again when the user tries the functions on the app.

Phase III:

TBA
