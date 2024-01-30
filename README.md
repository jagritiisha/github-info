# GitHub user-info

## Problem Statement
Display a GitHub user's profile, including their repositories with the functionality to paginate and search through them.

## How to run the project
Run index.html in your browser to view the project, pass the username as a query parameter to the url to view the profile of the user. For example, to view the profile of the user `user1`, run `index.html?username=user1` in your browser.

## JS Functions
- fetchGitHubProfile(username) is an async function that fetches the user's data and repositories from GitHub's API, then calls displayUserProfile(userData), displayRepos(), and setupPagination().
- displayUserProfile(userData) takes in the user's data as an argument and generates HTML to display the user's profile, then sets the innerHTML of the userProfile div to that HTML.
- displayRepos(repos = allRepos) takes in an array of repositories, defaults to allRepos if no argument is provided, and generates HTML to display the repositories.
- setupPagination(repos = allRepos) sets up the pagination by generating HTML for the page numbers.
changePage(pageNumber) changes the current page and re-displays the repositories and pagination.
- filterRepos() filters the repositories based on the search term from the search input field.
changeReposPerPage() changes the number of repositories displayed per page based on the selection from the dropdown.
