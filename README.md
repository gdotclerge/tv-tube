# Binge-Finder (Debugging Lab)

## Instructions

You and your team just crushed a project for one of your clients with time to spare! (Or so you thought)
As you were getting ready to celebrate one of your teammates expressed his frustration with the project and QUIT!
He decided to leave you with a little gift before his departure...

You now have a project with an unknown amount of bugs and your client is coming in for a presentation tonight *insert panicked emoji* Review the code that your team has written to discover and kill all the bugs in your application for a smooth presentation. Finish off with a round of celebratory drinks!


## Setup

* Clone this repository and cd into it.
* Run `npm install` or `yarn install` to install your dependencies.
* Run `npm start` or `yarn start` and the project will be running on localhost:3000.

## Deliverables

This is your end goal:

![Jest watch mode](./public/Debugging-Project-Demo.gif)


1. A user should be able to click on a show and have the details show up on the left.
2. A user should be able to search for a show.
3. A user should be able to filter the list of shows by their rating.
4. A user should be able to display seasons and episodes when a show is selected.


## BONUS

LAZY LOADING!! Your initial fetch only grabbed the most popular 240 shows on the API. Implement lazy loading to have your application do another fetch once it gets to the botton of the screen.

TIP change your fetch to reflect the page numbers example:
http://api.tvmaze.com/shows?page=1


## ERRORS

#### Adapter:
Missing a return in the first fetch.
Missing invocation on JSON method in second fetch.

#### Nav:
`Nav` is not receiving props.
All Components are lowercased.

#### App:
`handleFilter` method is setting state to wrong key in the state.
`handleSearch` is losing `THIS`. (either bind or use arrow function)

#### SelectedShowContainer:
`SelectedShowContainer` is exported but not as default.
Importing `Episode` with the incorrect local path.

#### TVShowList:
Accessing props incorrectly. (this.props vs props)
Not importing `TVShow`.
No `return` in `map` function (Implicit vs. Explicit return)

#### TVShow:
Not receiving props as an argument.
Not referencing image in props correctly.

#### Filter:
Not exporting component

`Episode` props named differently at `App`, `SelectedShowContainer` and `Episode` levels.
`SearchTerm` props named differently at `App` and `Nav` level.
