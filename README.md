# jira-selected-story-points
Displays the the combined story points of Jira issues that you have selected 

## Usage
Just create, or drag a new bookmark with the following code as the URL. 
`javascript: alert("Selected story points: " + $(".ghx-selected [title='Story Points']").map((i, s) => Number(s.innerText)).toArray().reduce((a,s) => a+s));`

## Example image
![Selected story points](http://i.imgur.com/DY3ez5m.png)

## Dependencies
Your Jira instance has to have jQuery as `$`, and your browser should support ES6

### Note
Tested on a newish version of Chrome and Safari, and some version of Jira. Your mileage might vary.
