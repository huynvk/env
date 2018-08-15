

## Define feature requirement

Create new story in back log as below:

```
User views Hello World page

AsA (As a)  
Users who open website

AC (Acceptance Criteria)  
- The text "HELLO WORLD" should display at center of the web site
- Spec follow screen design at http://design.shino.com/hello-world
- The text is always centered screen
- Clicking the text "HELLO WORLD" should trigger animation of changing text color to red, blue, green, and yellow

IC (Implementation Criteria)
- Website using blank HTML and javascript, no backend required
- Deployed as static site on google firebase cloud

PC (Provisional Criteria)  
- Mobile will be handled seperately
- No URL link required
- No caching required
- No performance index required

Notes  
N/A
```

## Sprint planing

1. Move the defined story from **backlog** to **TODO**

2. Estimate level of complexity. This story is agreed as Normal by the team --> set card label as Yellow

3. Assign action owner and due date

## Implementation

1. Move the defined story from **TODO** to **In Progress**  

2. Create new branch

* Select BitBucket > Create Branch
* On the BitBucket page, review the new branch name (user-views-hello-world-page) and click **Create Branch**
* New branch is created and updated in the card

3. Develop

* Checkout code to local PC

* Do development

* Commit 

* Push



3. Create Pull Request

* Click on the BitBucket branch on the Trello card to open BitBucket
* Select **Pull Request** > **Create Pull Request**
* Select to pull from new branch (user-views-hello-world-page) to master
* Enter the Product Owner and Sprint master as Reviewer
* Click **Create Pull Request**

## Review and close