The easiest way to create a new branch is with the following command. 

```bash
git checkout -b branch_name
```

This will create the new branch and *checkout* the new branch. Checkout means to point your repo to a branch. When you checkout a branch the state of your directory can change. To go back to the main branch us `git checkout main`.

## Branches as experiments
I like to use branches as experiments. As an example: I've been working on a simple math library for R. I've written functions to add and multiply 2 numbers. That might look something like this:

```r
add <- function (a, b) {
	a + b
}
```

What if we want that function to add all the numbers in a vector of numbers. *This is a very contrived example, don't worry about understanding the methods we are using within the code.*

It is a good idea to create a new branch to work on this new feature. This ensures that we don't mess up the code within our *main* branch.

```bash
git checkout -b feat_add
```

We've created a new branch called `feat_add` to create this new logic. Now we'll change the add function to look something like this:

```r
add <- function (x) {
	# x must be a vector
	Reduce(`+`, x)
}
```

Cool. We've tested this code, it works. Let's push it up to to GitHub so our collaborators can review the code. Since we are working on a branch that doesn't yet exist on GitHub we need to add a few additional bits of info with our push command. This will create the branch in GitHub.

```r
# push to origin from feat_add
git push -u origin feat_add
```

### Merge into main
Great, our collaborators think it is a good addition to our package so let's merge the code back into the *main* branch

```bash
# checkout the master branch
git checkout master

# then merge the feat_add branch
git merge master
```

The code is now integrated with the main branch. Notice that the code actually did change in Visual Studio Code.

Now we need to push the code to our remote main branch (to the origin).

```bash
# make sure you are on master
git push
```

## Merging on GitHub
The merging workflow we just did locally can be done on GitHub. So, let's make the same change to our multiply function on a new branch called `feat_multiply`

```bash
# create and checkout branch
git checkout -b feat_multiply
```

Now add change the code:

```r
multiply <- function (x) {
	# x must be a vector
	Reduce(`*`, x)
}
```

And push to GitHub:

```bash
git push -u origin feat_multiply
```

Great. We have a new branch on GitHub. Our collaborators agree that it is a good feature to include. Now let's run the merge workflow on GitHub. I'm not really going to explain that here, please watch the video to see how it works. 

Once the code is merged our origin is now 1 commit ahead of our main branch. To sync them run `git pull`. 

## Let's check the history
Now we can check the history with `git log`. 